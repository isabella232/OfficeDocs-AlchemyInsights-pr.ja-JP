---
title: Azure AD Connect でパスワードの書き戻しを有効にする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093360"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="8c5f0-102">Azure AD Connect でパスワードの書き戻しを有効にする</span><span class="sxs-lookup"><span data-stu-id="8c5f0-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="8c5f0-103">セルフサービスのパスワード リセットの書き戻しを有効にするには、まず Azure AD Connect で書き戻しを有効にします。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="8c5f0-104">Azure AD Connect サーバーから、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="8c5f0-105">Azure AD Connect サーバーにサインインし、**Azure AD Connect** 構成ウィザードを開始します。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="8c5f0-106">[**ようこそ**] ページで、[**構成**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="8c5f0-107">**[追加のタスク]** ページで、**[同期オプションのカスタマイズ]** を選択し、**[次へ]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="8c5f0-108">**[Azure AD に接続]** ページで、Azure テナントのグローバル管理者の資格情報を入力して、**[次へ]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="8c5f0-109">[**ディレクトリの接続**] ページと[**ドメインと OU のフィルタ リング**] ページで、[**次へ**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="8c5f0-110">**[オプション機能]** ページで、**[パスワードの書き戻し]** の横のボックスを選択し、**[次へ]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="8c5f0-111">[**構成の準備完了**] ページで[**構成**] をクリックし、処理が完了するのを待ちます。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="8c5f0-112">構成の完了が表示されたら、[**終了**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="8c5f0-113">Azure AD Connect でパスワードの書き戻しが有効にして、書き戻し用に Azure AD SSPR を構成します。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="8c5f0-114">SSPR でパスワードの書き戻しを有効にするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="8c5f0-115">グローバル管理者アカウントを使用して Azure ポータルにサインインします。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="8c5f0-116">[**Azure Active Directory**] を検索して選択し、[**パスワードのリセット**] をクリックして、[**オンプレミスの統合**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="8c5f0-117">[**オンプレミスのディレクトリにパスワードをライトバックしますか?**] のオプションを [**はい**] に設定します。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="8c5f0-118">[**パスワードをリセットせずにアカウントのロックを解除することをユーザーに許可しますか?**] オプションを [**はい**] に設定します。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="8c5f0-119">準備ができたら、[**保存**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-119">When ready, click **Save**.</span></span>

<span data-ttu-id="8c5f0-120">詳細については、「[オンプレミス環境への Azure Active Directory セルフサービスのパスワード リセットの書き戻しを有効にする](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="8c5f0-121">管理者が Azure ポータルでユーザーのパスワードをリセットしたとき、そのユーザーがフェデレーションされているかパスワードのハッシュが同期されている場合、パスワードがオンプレミスに書き戻されます。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="8c5f0-122">この機能には Azure プレミアム ライセンス (P1 または P2) が必要であり、現在 Office 管理ポータルではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c5f0-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>

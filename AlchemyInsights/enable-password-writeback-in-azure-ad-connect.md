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
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709732"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="2e935-102">Azure AD Connect でパスワードの書き戻しを有効にする</span><span class="sxs-lookup"><span data-stu-id="2e935-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="2e935-103">セルフサービスのパスワード リセットの書き戻しを有効にするには、まず Azure AD Connect で書き戻しを有効にします。</span><span class="sxs-lookup"><span data-stu-id="2e935-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="2e935-104">Azure AD Connect サーバーから、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="2e935-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="2e935-105">Azure AD Connect サーバーにサインインし、**Azure AD Connect** 構成ウィザードを開始します。</span><span class="sxs-lookup"><span data-stu-id="2e935-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="2e935-106">[**ようこそ**] ページで、[**構成**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="2e935-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="2e935-107">**[追加のタスク]** ページで、**[同期オプションのカスタマイズ]** を選択し、**[次へ]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="2e935-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="2e935-108">**[Azure AD に接続]** ページで、Azure テナントのグローバル管理者の資格情報を入力して、[次へ] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="2e935-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="2e935-109">[**ディレクトリの接続**] ページと[**ドメインと OU のフィルタ リング**] ページで、[**次へ**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="2e935-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="2e935-110">**[オプション機能]** ページで、**[パスワードの書き戻し]** の横のボックスを選択し、**[次へ]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="2e935-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="2e935-111">[**構成の準備完了**] ページで[**構成**] をクリックし、処理が完了するのを待ちます。</span><span class="sxs-lookup"><span data-stu-id="2e935-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="2e935-112">構成の完了が表示されたら、[**終了**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="2e935-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="2e935-113">Azure AD Connect でパスワードの書き戻しが有効になったら、書き戻し用に Azure AD SSPR を構成します。</span><span class="sxs-lookup"><span data-stu-id="2e935-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="2e935-114">SSPR でパスワードの書き戻しを有効にするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="2e935-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="2e935-115">グローバル管理者アカウントを使用して Azure ポータルにサインインします。</span><span class="sxs-lookup"><span data-stu-id="2e935-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="2e935-116">[**Azure Active Directory **] を検索して選択し、[**パスワードのリセット**] をクリックして、[**オンプレミスの統合**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="2e935-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="2e935-117">[**オンプレミスのディレクトリにパスワードをライトバックしますか?**] のオプションを [**はい**] に設定します。</span><span class="sxs-lookup"><span data-stu-id="2e935-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="2e935-118">[**パスワードをリセットせずにアカウントのロックを解除することをユーザーに許可しますか?**] オプションを [**はい**] に設定します。</span><span class="sxs-lookup"><span data-stu-id="2e935-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="2e935-119">準備ができたら、[**保存**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="2e935-119">When ready, click **Save**.</span></span>

<span data-ttu-id="2e935-120">詳細については、「[オンプレミス環境への Azure Active Directory セルフサービスのパスワード リセットの書き戻しを有効にする](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2e935-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

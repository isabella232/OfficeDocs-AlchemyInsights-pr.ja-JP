---
title: パスワード同期のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 2b0a1527ab1b16f56a97891445a2dcb4570302f5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533812"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="a8290-102">パスワード同期のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="a8290-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="a8290-103">Azure AD Connect バージョン 1.1.614.0 以降とパスワードが同期されないという問題をトラブルシューティングするには:</span><span class="sxs-lookup"><span data-stu-id="a8290-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="a8290-104">[**管理者として実行**] オプションを使用して、Azure AD Connect サーバーで新しい Windows PowerShell セッションを開きます。</span><span class="sxs-lookup"><span data-stu-id="a8290-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="a8290-105">**Set-ExecutionPolicy RemoteSigned** または **Set-ExecutionPolicy Unrestricted** を実行します。</span><span class="sxs-lookup"><span data-stu-id="a8290-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="a8290-106">Azure AD Connect ウィザードを開始します。</span><span class="sxs-lookup"><span data-stu-id="a8290-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="a8290-107">**[追加のタスク]** ページに移動し、**[トラブルシューティング]** を選択して **[次へ]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a8290-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span>

5. <span data-ttu-id="a8290-108">[トラブルシューティング] ページで、PowerShell の [**起動してトラブルシューティングを開始する**] メニューをクリックします。</span><span class="sxs-lookup"><span data-stu-id="a8290-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="a8290-109">メイン メニューで、[**パスワード同期のトラブルシューティング**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a8290-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="a8290-110">サブメニューで、[**パスワード同期がまったく動作しない**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a8290-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="a8290-111">**トラブルシューティング タスクの結果を理解する**</span><span class="sxs-lookup"><span data-stu-id="a8290-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="a8290-112">トラブルシューティング タスクでは、次のチェックが実行されます。</span><span class="sxs-lookup"><span data-stu-id="a8290-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="a8290-113">Azure AD テナントのパスワード同期機能が有効になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a8290-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="a8290-114">Azure AD Connect サーバーがステージング モードではないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="a8290-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="a8290-115">(既存の Active Directory フォレストに対応する) 既存のオンプレミス Active Directory コネクタごとに、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="a8290-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="a8290-116">パスワード同期機能が有効になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a8290-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="a8290-117">Windows アプリケーション イベント ログでパスワード同期ハートビート イベントを検索します。</span><span class="sxs-lookup"><span data-stu-id="a8290-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="a8290-118">オンプレミスの Active Directory コネクタの下にある Active Directory ドメインごとに、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="a8290-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="a8290-119">Azure AD Connect サーバーからドメインにアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a8290-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="a8290-120">オンプレミスの Active Directory コネクタで使用される Active Directory ドメイン サービス (AD DS) アカウントに、正しいユーザー名、パスワード、およびパスワードの同期に必要なアクセス許可があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a8290-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="a8290-121">パスワード同期のトラブルシューティングの詳細については、「[Azure AD Connect 同期によるパスワード同期のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8290-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  
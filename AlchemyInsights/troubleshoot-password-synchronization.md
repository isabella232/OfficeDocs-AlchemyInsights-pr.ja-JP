---
title: パスワード同期のトラブルシューティングを行う
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477038"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="8b8a7-102">パスワード同期のトラブルシューティングを行う</span><span class="sxs-lookup"><span data-stu-id="8b8a7-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="8b8a7-103">パスワードがないと Azure AD 接続バージョン 1.1.614.0 の同期またはそれ以降の問題をトラブルシューティングするには。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="8b8a7-104">**管理者として実行**オプションを使用して、Azure AD 接続サーバー上の新しい Windows PowerShell セッションを開きます。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="8b8a7-105">**セット ExecutionPolicy RemoteSigned**または**無制限に設定 ExecutionPolicy**を実行します。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="8b8a7-106">Azure AD 接続ウィザードを起動します。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="8b8a7-107">移動、\* \* 追加のタスク \* \* ページで、[\* \* トラブルシューティング \* \*、[**次へ**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="8b8a7-108">[トラブルシューティング] ページで、PowerShell での**トラブルシューティングを開始するのには起動**メニューをクリックします。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="8b8a7-109">メイン メニューでは、**パスワード同期のトラブルシューティングを行う**を選択します。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="8b8a7-110">サブ ・ メニューには、**パスワード同期がまったく動作しない**を選択します。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="8b8a7-111">**トラブルシューティングのタスクの結果を理解します。**</span><span class="sxs-lookup"><span data-stu-id="8b8a7-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="8b8a7-112">トラブルシューティングのタスクには、次のチェックが実行されます。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="8b8a7-113">Azure AD テナントのパスワード同期機能が有効になっていることを検証します。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="8b8a7-114">Azure AD 接続サーバーはステージング モードでないことを検証します。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="8b8a7-115">各既存のオンプレミス Active Directory コネクタ (これは、既存の Active Directory フォレストに相当します)。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="8b8a7-116">パスワード同期機能が有効になっていることを検証します。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="8b8a7-117">Windows アプリケーション イベント ログ内のパスワード同期パルス イベントを検索します。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="8b8a7-118">: オンプレミスの Active Directory コネクタの下にある Active Directory ドメインごとに</span><span class="sxs-lookup"><span data-stu-id="8b8a7-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="8b8a7-119">ドメインは、Azure AD 接続サーバーから到達できることを検証します。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="8b8a7-120">オンプレミスの Active Directory コネクタが使用する Active Directory ドメイン サービス (AD DS) アカウントが正しいユーザー名、パスワード、およびパスワード同期に必要なアクセス許可を持つことを検証します。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="8b8a7-121">パスワード同期のトラブルシューティングの詳細については、 [Azure AD 接続の同期がパスワード同期のトラブルシューティング](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b8a7-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  


---
title: "\"アクセスが拒否されました\" メッセージのトラブルシューティング"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759805"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="1e64c-102">"アクセスが拒否されました" メッセージのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="1e64c-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="1e64c-p101">ユーザーが SharePoint の共有フォルダーにアクセスしようとしたときに「アクセスが拒否されました」メッセージを受け取った場合、サイト コレクション管理者が「制限付きアクセスのユーザーのアクセス許可ロックダウン モード」を有効にしている可能性があります。これを無効にするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="1e64c-p101">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="1e64c-105">サイトを参照して、[設定] アイコンをクリックし、[**サイト設定**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="1e64c-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="1e64c-106">[**サイト コレクションの管理**] で、[**サイト コレクションの機能**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="1e64c-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="1e64c-107">[**制限付きアクセスのユーザーのアクセス許可ロックダウン モード**] の横にある [**非アクティブ化**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="1e64c-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="1e64c-p102">"アクセスが拒否されました" メッセージは、サイトが発行サイトである場合に共有フォルダーを参照しようとしたときにも発生します。詳細については、[共有フォルダーにアクセスしようとしたときに表示される "アクセスが拒否されました" エラー メッセージに関する記事](https://go.microsoft.com/fwlink/?linkid=2004317)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e64c-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="1e64c-p103">ユーザーがアクセス依頼を表示しようとしたときに "アクセスが拒否されました" メッセージを受け取った場合、そのユーザーをサイト コレクション管理者またはサイトの所有者グループのメンバーとして追加する必要があります。詳細については、[アクセス依頼リストにアクセスしようとしたときに表示される "アクセスが拒否されました" エラー メッセージに関する記事](https://go.microsoft.com/fwlink/?linkid=2004220)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e64c-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="1e64c-112">ユーザーがオンプレミスの Active Directory から削除され、再度追加された後に "アクセスが拒否されました" メッセージを受け取った場合は、[ユーザー アカウントを Microsoft 365 に同期しようとしたときに表示される "アクセスが拒否されました" エラー メッセージに関する記事](https://go.microsoft.com/fwlink/?linkid=2004318)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e64c-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  


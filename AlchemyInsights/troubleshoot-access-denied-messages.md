---
title: アクセス拒否のメッセージをトラブルシューティングします。
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476545"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="41915-102">アクセス拒否のメッセージをトラブルシューティングします。</span><span class="sxs-lookup"><span data-stu-id="41915-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="41915-p101">共有フォルダーに"アクセスが拒否されました"というメッセージは、他の場合、サイト コレクションの管理者が有効にしている「アクセスが制限されたユーザーのアクセス許可のロックダウン モード」これを無効にします。</span><span class="sxs-lookup"><span data-stu-id="41915-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="41915-105">サイトを参照、設定アイコンをクリックし、[**サイトの設定**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="41915-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="41915-106">[サイト コレクションの管理] で、[サイト コレクションの機能] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="41915-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="41915-107">**アクセス制限されたユーザーのアクセス許可のロックダウン モード**の横にある**非アクティブ化**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="41915-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="41915-p102">アクセス拒否のメッセージも発生する可能性が共有フォルダーの場合は、サイトは、発行サイトです。情報は[共有フォルダーにアクセスするとき、アクセスが拒否されました](https://go.microsoft.com/fwlink/?linkid=2004317)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41915-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="41915-p103">場合は、「アクセス拒否」メッセージは、アクセス要求を表示しようとするとき、誰かが、ユーザーをサイト コレクションの管理者またはサイトの所有者グループのメンバーとして追加する必要があります。詳細については、[アクセス権の要求] ボックスの一覧へのアクセス拒否](https://go.microsoft.com/fwlink/?linkid=2004220)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41915-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="41915-112">ユーザーは、社内の Active Directory から削除され、再び追加し、された後に、"アクセスが拒否されました"というメッセージを取得、する場合は、[ユーザー アカウントが Office 365 に同期されるとき、アクセスが拒否されました](https://go.microsoft.com/fwlink/?linkid=2004318)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41915-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  


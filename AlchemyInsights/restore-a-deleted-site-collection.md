---
title: 削除されたサイトを復元する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: d37fd903c91c8cd6ac6137e815cb253f7edb4494
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912680"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="d1c34-102">削除されたサイトを復元する</span><span class="sxs-lookup"><span data-stu-id="d1c34-102">Restore a deleted site</span></span>

<span data-ttu-id="d1c34-p101">管理者が SharePoint サイトを削除すると、サイト コレクションのごみ箱に入れられ、93 日間保管されてから完全に削除されます。サイトを復元するには、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1c34-p101">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site:</span></span>
  
1. <span data-ttu-id="d1c34-105">新しい SharePoint Online 管理センター のリボンにある **[ごみ箱]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d1c34-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="d1c34-106">復元するサイト コレクションの横にあるチェック ボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="d1c34-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="d1c34-107">**[削除したアイテムを復元]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d1c34-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="d1c34-p102">削除したコミュニケーション サイトを復元する場合は、新しい SharePoint 管理センターを使用できます。それ以外の場合は、Microsoft PowerShell を使用する必要があります。Microsoft 365 グループに属するサイトを復元する場合は、そのグループを Exchange 管理センターで復元する必要があります。グループは、削除後 30 日経過するまで復元可能です。</span><span class="sxs-lookup"><span data-stu-id="d1c34-p102">To restore a deleted communication site, you can use the new SharePoint admin center. Otherwise, you need to use Microsoft PowerShell. To restore a site that belongs to an Microsoft 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  


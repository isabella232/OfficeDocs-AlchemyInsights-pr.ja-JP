---
title: 削除されたサイト コレクションを復元する
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: b3c72033dfcc093dd0c2837d2866c6a78d64449c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476617"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="d8868-102">削除されたサイト コレクションを復元する</span><span class="sxs-lookup"><span data-stu-id="d8868-102">Restore a deleted site collection</span></span>

<span data-ttu-id="d8868-p101">管理者が従来のサイト コレクションを削除すると、そのコレクションはサイト コレクションのごみ箱に入れられます。削除されたコレクションは、このごみ箱で 93 日間保持されてから、完全に削除されます。サイト コレクションを復元するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="d8868-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="d8868-105">従来の SharePoint 管理センターで、リボンにある **[ごみ箱]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d8868-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="d8868-106">復元するサイト コレクションの横にあるチェック ボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="d8868-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="d8868-107">**[削除したアイテムを復元]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d8868-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="d8868-p102">削除したコミュニケーション サイトを復元する場合は、プレビュー版の新しい SharePoint 管理センターを使用できます。それ以外の場合は、PowerShell を使用する必要があります。Office 365 グループに属するサイトを復元する場合は、そのグループを Exchange 管理センターで復元する必要があります。グループは、削除後 30 日経過するまで復元可能です。</span><span class="sxs-lookup"><span data-stu-id="d8868-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  


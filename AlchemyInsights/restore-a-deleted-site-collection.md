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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297625"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="0fd32-102">削除されたサイト コレクションを復元する</span><span class="sxs-lookup"><span data-stu-id="0fd32-102">Restore a deleted site collection</span></span>

<span data-ttu-id="0fd32-p101">管理者は、従来のサイト コレクションを削除、ごみ箱を恒久的に削除される前に、の 93 日間保存されているサイト コレクション内に置かれます。サイト コレクションを復元するには。</span><span class="sxs-lookup"><span data-stu-id="0fd32-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="0fd32-105">クラシック SharePoint 管理センターで、リボンの [**ごみ箱**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0fd32-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="0fd32-106">復元するサイト コレクションの横にあるチェック ボックスを選択します。</span><span class="sxs-lookup"><span data-stu-id="0fd32-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="0fd32-107">**削除済みアイテムを復元**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0fd32-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="0fd32-p102">削除されたコミュニケーション サイトを復元するには、新しい SharePoint 管理センターのプレビューを使用できます。それ以外の場合、PowerShell を使用する必要があります。Office 365 のグループに属しているサイトを復元するには、Exchange 管理センターでのグループを復元する必要があります。削除後 30 日間のグループを復元できます。</span><span class="sxs-lookup"><span data-stu-id="0fd32-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  


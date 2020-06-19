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
ms.openlocfilehash: 7c2ae754c86a3502092b622c55d18f3f4006bf8b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582240"
---
# <a name="restore-a-deleted-site"></a>削除されたサイトを復元する

When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site:
  
1. 新しい SharePoint Online 管理センター のリボンにある **[ごみ箱]** をクリックします。 
    
2. 復元するサイト コレクションの横にあるチェック ボックスをオンにします。
    
3. **[削除したアイテムを復元]** をクリックします。
    
To restore a deleted communication site, you can use the new SharePoint admin center. Otherwise, you need to use Microsoft PowerShell. To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.
  


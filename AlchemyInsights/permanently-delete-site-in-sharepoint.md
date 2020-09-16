---
title: SharePoint のサイトを完全に削除する
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771726"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>SharePoint のサイトを完全に削除する

(サイトを再作成するために) 削除したサイトの URL を再利用する場合、または使用しなくなったサイトを完全に削除する場合には、新しい SharePoint 管理センターの **[完全に削除]** を使用できます。 

1. [新しい SharePoint 管理センターの [削除されたサイト] ページ](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)に移動し、組織の管理者権限が付与されているアカウントでサインインします。 

2. 左側の列で、サイトをクリックします。 

3. **[完全に削除]** をクリックします。 

**注**: 新しい SharePoint 管理センターからは、グループが接続されているサイトを完全に削除することはできません。 [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) を代わりに使用する必要があります。  

詳しくは、「[サイトを完全に削除する](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site)」を参照してください。 

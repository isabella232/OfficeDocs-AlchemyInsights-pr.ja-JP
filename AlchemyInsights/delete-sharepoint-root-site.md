---
title: SharePoint のルート サイトを削除する
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
- "9003017"
- "5727"
ms.openlocfilehash: d33029b6fe333b38cee7dba66ba4a5044248f174
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679905"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="2709d-102">SharePoint のルート サイトを削除する</span><span class="sxs-lookup"><span data-stu-id="2709d-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="2709d-103">SharePoint のルートサイトの削除は **サポートされていません。**</span><span class="sxs-lookup"><span data-stu-id="2709d-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="2709d-104">ルート サイトが既に削除されている場合、ユーザーがサイトにアクセスしようとすると「404 ファイルが見つかりません」エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="2709d-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="2709d-105">解決するには、新しい SharePoint 管理センターから [[削除されたサイト](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)] ページに移動してサイトを復元し、ルート サイトを選択して [復元] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="2709d-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="2709d-106">ルート サイトを削除する代わりに、ルート サイトが復元されたら、新しい SharePoint 管理センターから[サイトの置き換え](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)を使用します。</span><span class="sxs-lookup"><span data-stu-id="2709d-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="2709d-107">詳細については、「[ルート サイトのモダン化](https://docs.microsoft.com/sharepoint/modern-root-site)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2709d-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>
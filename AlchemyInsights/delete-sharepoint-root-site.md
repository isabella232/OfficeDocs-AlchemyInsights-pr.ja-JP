---
title: SharePoint のルート サイトを削除する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: 849c5c58ab4688130d71baffac8fe39eddf92f18
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815476"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="44c03-102">SharePoint のルート サイトを削除する</span><span class="sxs-lookup"><span data-stu-id="44c03-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="44c03-103">SharePoint のルートサイトの削除は **サポートされていません。**</span><span class="sxs-lookup"><span data-stu-id="44c03-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="44c03-104">ルート サイトが既に削除されている場合、ユーザーがサイトにアクセスしようとすると「404 ファイルが見つかりません」エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="44c03-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="44c03-105">解決するには、新しい SharePoint 管理センターから [[削除されたサイト](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)] ページに移動してサイトを復元し、ルート サイトを選択して [復元] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="44c03-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="44c03-106">ルート サイトを削除する代わりに、ルート サイトが復元されたら、新しい SharePoint 管理センターから[サイトの置き換え](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)を使用します。</span><span class="sxs-lookup"><span data-stu-id="44c03-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="44c03-107">詳細については、「[ルート サイトのモダン化](https://docs.microsoft.com/sharepoint/modern-root-site)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44c03-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>
---
title: SharePoint のルート サイトを削除する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: 0a1f4adc6245cfe89251df28d2786154dcca8f56
ms.sourcegitcommit: 172f26bd1eeed5251c22d4e311065cf3284fef4b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/27/2020
ms.locfileid: "44404981"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="7956c-102">SharePoint のルート サイトを削除する</span><span class="sxs-lookup"><span data-stu-id="7956c-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="7956c-103">SharePoint のルート サイトの削除はサポートされておらず、Microsoft はルート サイトの削除防止を段階的に展開しています。</span><span class="sxs-lookup"><span data-stu-id="7956c-103">Deleting the SharePoint root site is not supported and Microsoft is gradually rolling out prevention of root site deletion.</span></span>

- <span data-ttu-id="7956c-104">ルート サイトが既に削除されている場合、ユーザーがサイトにアクセスしようとすると、「**404 ファイルが見つかりません**」エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="7956c-104">If the root site has already been deleted, users will experience a **404 File Not Found** error when trying to access the site.</span></span>
- <span data-ttu-id="7956c-105">新しい SharePoint 管理センターから [[削除されたサイト](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)] ページに移動して**サイトを復元**し、ルート サイトを選択して [**復元**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7956c-105">**Restore the site** from the new SharePoint admin center by going to the [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) page, select the root site and click **Restore**.</span></span>
- <span data-ttu-id="7956c-106">ルート サイトを削除する代わりに、ルート サイトが復元されたら、新しい SharePoint 管理センターから[置換サイト](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)を使用します。</span><span class="sxs-lookup"><span data-stu-id="7956c-106">Instead of deleting the root site, use the [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="7956c-107">詳細については、「[ルート サイトを最新化する](https://docs.microsoft.com/sharepoint/modern-root-site)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7956c-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span>

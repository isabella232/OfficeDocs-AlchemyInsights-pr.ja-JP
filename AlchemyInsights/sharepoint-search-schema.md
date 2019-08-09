---
title: SharePoint Online で検索スキーマを管理する
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f49195bec64f115063ccfb5256e27fbecd4a54f6
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270116"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="52414-102">SharePoint Online で検索スキーマを管理する</span><span class="sxs-lookup"><span data-stu-id="52414-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="52414-103">検索スキーマは、ユーザーが検索できる対象、ユーザーが検索できる方法、検索結果を検索 web サイトに提示する方法を制御します。</span><span class="sxs-lookup"><span data-stu-id="52414-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="52414-104">方法については[、「SharePoint Online で検索スキーマを管理](https://docs.microsoft.com/sharepoint/manage-search-schema)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52414-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="52414-105">検索スキーマを変更します。</span><span class="sxs-lookup"><span data-stu-id="52414-105">Change the search schema.</span></span>
- <span data-ttu-id="52414-106">管理プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="52414-106">Create managed properties.</span></span>
- <span data-ttu-id="52414-107">クロールされたマップのクロールされたプロパティを管理プロパティにマップします。</span><span class="sxs-lookup"><span data-stu-id="52414-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="52414-108">検索スキーマの管理に関しては、次の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="52414-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="52414-109">スキーマの変更時に**アプリケーションが一時停止**したことを示す警告が表示された場合は、サービスの保守が行われている限り、これは一時的なものになります。</span><span class="sxs-lookup"><span data-stu-id="52414-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="52414-110">24時間以上経過しても警告が表示される場合は、サポートケースをログに記録してください。</span><span class="sxs-lookup"><span data-stu-id="52414-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="52414-111">管理プロパティを変更するか、新しい管理プロパティを追加すると、変更はコンテンツが再クロールされた後にのみ有効になります。</span><span class="sxs-lookup"><span data-stu-id="52414-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="52414-112">SharePoint Online では、クロールは、定義されたクロールスケジュールに基づいて自動的に行われます。</span><span class="sxs-lookup"><span data-stu-id="52414-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="52414-113">変更がクロールされるようにするには、[リストまたはライブラリのインデックスの再作成を](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)具体的に要求できます。</span><span class="sxs-lookup"><span data-stu-id="52414-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="52414-114">検索スキーマの完全な概要については、「[検索スキーマ](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)の概要」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52414-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 



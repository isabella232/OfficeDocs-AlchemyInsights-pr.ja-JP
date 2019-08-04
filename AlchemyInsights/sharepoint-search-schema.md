---
title: SharePoint Online の検索辞書を管理する
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 8aba36b20098ca7b2ad2564946b4696f3c5ad34a
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059150"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="b4f31-102">SharePoint Online で検索スキーマを管理する</span><span class="sxs-lookup"><span data-stu-id="b4f31-102">Manage the search schema in SharePoint Online</span></span>

<span data-ttu-id="b4f31-103">検索スキーマでは、検索対象、検索方法、検索 Web サイトに検索結果を表示する方法を制御します。</span><span class="sxs-lookup"><span data-stu-id="b4f31-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="b4f31-104">次の方法の詳細については、「[SharePoint Online で検索スキーマを管理する](https://docs.microsoft.com/sharepoint/manage-search-schema)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4f31-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="b4f31-105">検索スキーマを変更する。</span><span class="sxs-lookup"><span data-stu-id="b4f31-105">Manage the search schema</span></span>
- <span data-ttu-id="b4f31-106">管理プロパティを作成する。</span><span class="sxs-lookup"><span data-stu-id="b4f31-106">Create managed properties</span></span>
- <span data-ttu-id="b4f31-107">クロールされたマップのクロールされたプロパティを管理プロパティにマップする。</span><span class="sxs-lookup"><span data-stu-id="b4f31-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="b4f31-108">検索スキーマの管理については、次の点にご注意ください。</span><span class="sxs-lookup"><span data-stu-id="b4f31-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="b4f31-109">スキーマの変更を行うときに **アプリケーションが一時停止しています** という警告を受け取った場合、これはサービスの保守を行っている最中の一時的な状態に過ぎません。</span><span class="sxs-lookup"><span data-stu-id="b4f31-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="b4f31-110">24 時間以上経過しても警告が表示される場合は、サポート ケースを記録してください。</span><span class="sxs-lookup"><span data-stu-id="b4f31-110">If more than 24 hours have passed and you're still experiencing the issue, please log a support ticket.</span></span>
- <span data-ttu-id="b4f31-111">管理プロパティを変更するか、新しい管理プロパティを追加すると、その変更はコンテンツが再クロールされた後でのみ有効になります。</span><span class="sxs-lookup"><span data-stu-id="b4f31-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="b4f31-112">SharePoint Online では、定義されたクロール スケジュールに従って、クロールが自動的に行われます。</span><span class="sxs-lookup"><span data-stu-id="b4f31-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="b4f31-113">変更が確実にクロールされるよう、[リストやライブラリのインデックスの再作成を具体的に要求](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)することができます。</span><span class="sxs-lookup"><span data-stu-id="b4f31-113">To make sure that your changes are crawled and reindexed, you can specifically request a reindexing of the list or library.</span></span> 

<span data-ttu-id="b4f31-114">検索スキーマの完全な概要については、「[Introducing Search Schema for SharePoint (SharePoint の検索スキーマの概要)](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4f31-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 



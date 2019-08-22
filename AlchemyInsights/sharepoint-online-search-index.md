---
title: SharePoint Online での検索
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507636"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="2ca2f-102">SharePoint Online でのコンテンツのクロールとインデックス作成</span><span class="sxs-lookup"><span data-stu-id="2ca2f-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="2ca2f-103">SharePoint Online で検索する内容を検索するには、コンテンツをクロールして、検索インデックスに追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="2ca2f-104">コンテンツは、定義済みのクロールスケジュールに基づいて自動的にクロールされます (クロールスケジュールを変更することはできません)。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="2ca2f-105">クローラーは、最後にクロールされて以降に変更が加えられたコンテンツを取得して、インデックスを更新します。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="2ca2f-106">コンテンツがクロールされ、インデックスが更新されるようにするには、次の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="2ca2f-107">[サイトコンテンツを検索](https://docs.microsoft.com/sharepoint/make-site-content-searchable)可能にすることで、コンテンツを検出できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="2ca2f-108">管理プロパティを変更した場合、またはクロールされたプロパティと管理プロパティのマッピングを変更した場合、変更が検索インデックスに反映されるようにするには、サイトを再クロールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="2ca2f-109">変更は検索スキーマで行われ、実際のサイトでは変更されないため、クローラーは自動的にサイトを再インデックス付けすることはありません。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="2ca2f-110">詳細については、「[サイト、ライブラリ、またはリストのクロールとインデックス再作成を手動で要求](https://docs.microsoft.com/sharepoint/crawl-site-conten)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="2ca2f-111">クロールと完全な再インデックスを手動で要求した後、少なくとも24時間待って、問題が発生しているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="2ca2f-112">クロールを開始してから、フルインデックスを作成してから24時間以上経過した場合は、サポートケースをログに記録してください。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="2ca2f-113">多くの場合、すでに解決策に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="2ca2f-114">解決策を完成させるために少なくとも 24 時間を与えてください。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2ca2f-115">サイト、ドキュメント (ライブラリ)、またはリストが削除されていても検索結果に表示される場合は、アクセスしようとしたときに**エラー404ファイルが見つからない**ことをユーザーに通知する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="2ca2f-116">この問題は、詳細な調査のサポートケースとしてログに記録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ca2f-116">This issue should be logged as a support case for further investigation.</span></span> 




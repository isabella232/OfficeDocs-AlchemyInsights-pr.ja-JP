---
title: SharePoint Online での検索
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044048"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="ea341-102">SharePoint Online でのコンテンツのクロールとインデックス作成</span><span class="sxs-lookup"><span data-stu-id="ea341-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="ea341-103">ユーザーが SharePoint Online のコンテンツを検索できるようにするには、コンテンツをクロールし、検索インデックスに追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ea341-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="ea341-104">コンテンツは、事前に定義されたクロール スケジュールに基づいて自動的にクロールされます (クロール スケジュールは変更できません)。</span><span class="sxs-lookup"><span data-stu-id="ea341-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="ea341-105">クローラーは、最後にクロールを実行したとき以降に変更されたコンテンツを取得し、インデックスを更新します。</span><span class="sxs-lookup"><span data-stu-id="ea341-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="ea341-106">コンテンツがクロールされ、インデックスが更新されるようにするためには、次の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="ea341-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="ea341-107">コンテンツを見つけることができるよう、[サイト コンテンツを検索可能にします](https://docs.microsoft.com/sharepoint/make-site-content-searchable)。</span><span class="sxs-lookup"><span data-stu-id="ea341-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="ea341-108">管理プロパティを変更した場合や、クロールされたプロパティと管理プロパティのマッピングを変更した場合は、サイトを再クロールしないと、検索インデックスに変更内容が反映されません。</span><span class="sxs-lookup"><span data-stu-id="ea341-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="ea341-109">変更は検索スキーマ内で行われ、実際のサイトに対しては行われていないため、クローラーでサイトのインデックスが自動的に再作成されることはありません。</span><span class="sxs-lookup"><span data-stu-id="ea341-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="ea341-110">詳細については、「[サイトのクロールとインデックス再作成を手動で要求する](https://docs.microsoft.com/sharepoint/crawl-site-conten)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea341-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="ea341-111">手動によるクロールとインデックスの完全な再作成の要求後少なくとも 24 時間以上待ってから、問題が引き続き発生するかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="ea341-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="ea341-112">クロールとインデックスの完全な再作成の開始後 24 時間以上経過している場合は、サポート ケースを記録してください。</span><span class="sxs-lookup"><span data-stu-id="ea341-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="ea341-113">多くの場合、すでに解決策に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="ea341-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="ea341-114">解決策を完成させるために少なくとも 24 時間を与えてください。</span><span class="sxs-lookup"><span data-stu-id="ea341-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ea341-115">サイト、ドキュメント (ライブラリ)、またはリストを削除した後も検索結果に表示される場合、ユーザーがアクセスを試みると [**エラー 404 ファイルが見つかりません**] というエラーが表示されるはずです。</span><span class="sxs-lookup"><span data-stu-id="ea341-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="ea341-116">この問題は、詳細な調査のためにサポート ケースとして記録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ea341-116">This issue should be logged as a support case for further investigation.</span></span> 




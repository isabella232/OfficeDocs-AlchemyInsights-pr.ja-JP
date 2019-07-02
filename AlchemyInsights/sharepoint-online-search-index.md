---
title: SharePoint Online の検索辞書を管理する
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 5319c2f1edc3e61074301f039736d2aa96bda47b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35174468"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="6f45f-102">SharePoint Online での検索</span><span class="sxs-lookup"><span data-stu-id="6f45f-102">Microsoft Search in SharePoint Online</span></span>

<span data-ttu-id="6f45f-103">ユーザーが SharePoint Online のコンテンツを検索できるようにするには、コンテンツをクロールし、検索インデックスに追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6f45f-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="6f45f-104">コンテンツは、事前に定義されたクロール スケジュールに基づいて自動的にクロールされます (クロール スケジュールは変更できません)。</span><span class="sxs-lookup"><span data-stu-id="6f45f-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="6f45f-105">クローラーは、最後にクロールを実行したとき以降に変更されたコンテンツを取得し、インデックスを更新します。</span><span class="sxs-lookup"><span data-stu-id="6f45f-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="6f45f-106">コンテンツがクロールされ、インデックスが更新されるようにするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="6f45f-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="6f45f-107">コンテンツを見つけることができるよう、サイト コンテンツを検索可能にします。</span><span class="sxs-lookup"><span data-stu-id="6f45f-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="6f45f-108">詳細については、「[サイトのコンテンツを検索可能にする](https://docs.microsoft.com/sharepoint/make-site-content-searchable)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f45f-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="6f45f-109">管理プロパティを変更した場合や、クロールされたプロパティと管理プロパティのマッピングを変更した場合は、サイトを再クロールしないと、検索インデックスに変更内容が反映されません。</span><span class="sxs-lookup"><span data-stu-id="6f45f-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="6f45f-110">変更は検索スキーマ内で行われ、実際のサイトに対しては行われていないため、クローラーでサイトのインデックスが自動的に再作成されることはありません。</span><span class="sxs-lookup"><span data-stu-id="6f45f-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically reindex the list or the library.</span></span> 

<span data-ttu-id="6f45f-111">詳細については、「[サイトのクロールとインデックス再作成を手動で要求する](https://docs.microsoft.com/sharepoint/crawl-site-conten)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f45f-111">For more information, see [Manually request crawling and re-indexing of a site, a library or a listhttp://go.microsoft.com/fwlink/p/?LinkID=627457](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="6f45f-112">手動によるクロールとインデックスの完全な再作成の要求後少なくとも 24 時間以上待ってから、問題が引き続き発生するかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="6f45f-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="6f45f-113">クロールとインデックスの完全な再作成の開始後 24 時間以上経過している場合は、サポート ケースを記録してください。</span><span class="sxs-lookup"><span data-stu-id="6f45f-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="6f45f-114">多くの場合、すでに解決策に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="6f45f-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="6f45f-115">解決策を完成させるために少なくとも 24 時間を与えてください。</span><span class="sxs-lookup"><span data-stu-id="6f45f-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="6f45f-116">**重要**: サイト、ドキュメント (ライブラリ)、またはリストを削除した後も検索結果に表示される場合、ユーザーがアクセスを試みると [エラー 404 ファイルが見つかりません] というエラーが表示されるはずです。</span><span class="sxs-lookup"><span data-stu-id="6f45f-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="6f45f-117">この問題は、詳細な調査のためにサポート ケースとして記録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6f45f-117">This issue should be logged as a support case for further investigation.</span></span> 




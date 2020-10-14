---
title: SharePoint Online での検索
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f790efbe6ed445786933efa3fc980f974693d1d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770772"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="2fcbd-102">SharePoint Online でのコンテンツのクロールとインデックス作成</span><span class="sxs-lookup"><span data-stu-id="2fcbd-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="2fcbd-103">ユーザーが SharePoint Online のコンテンツを検索できるようにするには、コンテンツをクロールし、検索インデックスに追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2fcbd-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span>

- <span data-ttu-id="2fcbd-104">コンテンツを見つけることができるよう、[サイト コンテンツを検索可能にします](https://docs.microsoft.com/sharepoint/make-site-content-searchable)。</span><span class="sxs-lookup"><span data-stu-id="2fcbd-104">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="2fcbd-105">管理プロパティを変更した場合や、クロールされたプロパティと管理プロパティのマッピングを変更した場合は、サイトを再クロールしないと、検索インデックスに変更内容が反映されません。</span><span class="sxs-lookup"><span data-stu-id="2fcbd-105">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span>

- <span data-ttu-id="2fcbd-106">詳細については、「[サイトのクロールとインデックス再作成を手動で要求する](https://docs.microsoft.com/sharepoint/crawl-site-content)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fcbd-106">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span>

- <span data-ttu-id="2fcbd-107">手動によるクロールとインデックスの完全な再作成の要求後少なくとも 24 時間以上待ってから、問題が引き続き発生するかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="2fcbd-107">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span>

- <span data-ttu-id="2fcbd-108">クロールとインデックスの完全な再作成の開始後 24 時間以上経過している場合は、サポート ケースを記録してください。</span><span class="sxs-lookup"><span data-stu-id="2fcbd-108">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="2fcbd-109">多くの場合、すでに解決策に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="2fcbd-109">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="2fcbd-110">解決策を完成させるために少なくとも 24 時間を与えてください。</span><span class="sxs-lookup"><span data-stu-id="2fcbd-110">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="2fcbd-111">**重要**: サイト、ドキュメント (ライブラリ)、またはリストを削除した後も検索結果に表示される場合、ユーザーがアクセスを試みると「**エラー 404 ファイルが見つかりません**」というエラーが表示されるはずです。</span><span class="sxs-lookup"><span data-stu-id="2fcbd-111">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="2fcbd-112">この問題は、詳細な調査のためにサポート ケースとして記録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2fcbd-112">This issue should be logged as a support case for further investigation.</span></span>




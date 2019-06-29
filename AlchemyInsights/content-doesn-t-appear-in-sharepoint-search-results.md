---
title: SharePoint の検索結果にコンテンツが表示されない
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363816"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="e2e16-102">SharePoint の検索結果にコンテンツが表示されない</span><span class="sxs-lookup"><span data-stu-id="e2e16-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="e2e16-103">想定されるコンテンツが検索結果に表示されない場合は、次のトラブルシューティング手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="e2e16-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="e2e16-p101">想定されるコンテンツを含む**サイト**が、検索結果にコンテンツを表示するように設定されていることを確認します。「[検索結果でサイトにコンテンツを表示する](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)」の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="e2e16-p101">Check that the **site** that contains the expected content is set to allow content to appear in search results. Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="e2e16-p102">想定されるコンテンツを含む**リスト**または**ライブラリ**が、検索結果にコンテンツを表示するように設定されていることを確認します。「[検索結果にリストまたはライブラリのコンテンツを表示する](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)」の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="e2e16-p102">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results. Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="e2e16-p103">ページ、ドキュメント、またはカスタム ページ レイアウトが**メジャー バージョン**として公開されていることを確認します。「[SharePoint Online で検索がすべての結果を返さない](https://go.microsoft.com/fwlink/?linkid=874525)」の手順 3 を実行します。</span><span class="sxs-lookup"><span data-stu-id="e2e16-p103">Verify that the page, document, or custom page layout is published as a **Major version.** Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="e2e16-p104">ユーザーがコンテンツを表示するための**アクセス許可**を持っていることを確認します。「[SharePoint でのアクセス許可レベルについて](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels)」の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="e2e16-p104">Verify that the user has **permissions** to view the content. Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="e2e16-112">新しい管理プロパティを追加して検索スキーマを変更した場合、管理プロパティを編集した場合、または管理プロパティを削除した場合は、クロールを要求し、インデックスの再作成が必要になります。</span><span class="sxs-lookup"><span data-stu-id="e2e16-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="e2e16-113">[サイト、ライブラリ、またはリストのクロールとインデックス再作成を手動で要求](https://docs.microsoft.com/sharepoint/crawl-site-content)する手順に従って、コンテンツの**インデックスを再**作成します。</span><span class="sxs-lookup"><span data-stu-id="e2e16-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="e2e16-114">この処理には時間がかかることがあります。24時間待ってから結果を再度確認してください。</span><span class="sxs-lookup"><span data-stu-id="e2e16-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="e2e16-115">詳細については、「[サイトのコンテンツを検索](https://docs.microsoft.com/sharepoint/make-site-content-searchable)可能にする」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2e16-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  

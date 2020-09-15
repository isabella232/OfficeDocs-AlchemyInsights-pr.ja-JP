---
title: SharePoint の検索結果にコンテンツが表示されない
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713135"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="eee6a-102">SharePoint の検索結果にコンテンツが表示されない</span><span class="sxs-lookup"><span data-stu-id="eee6a-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="eee6a-103">想定されるコンテンツが検索結果に表示されない場合は、次のトラブルシューティング手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="eee6a-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="eee6a-p101">想定されるコンテンツを含む**サイト**が、検索結果にコンテンツを表示するように設定されていることを確認します。「[検索結果でサイトにコンテンツを表示する](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)」の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="eee6a-p101">Check that the **site** that contains the expected content is set to allow content to appear in search results. Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="eee6a-p102">想定されるコンテンツを含む**リスト**または**ライブラリ**が、検索結果にコンテンツを表示するように設定されていることを確認します。「[検索結果にリストまたはライブラリのコンテンツを表示する](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)」の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="eee6a-p102">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results. Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="eee6a-p103">ページ、ドキュメント、またはカスタム ページ レイアウトが**メジャー バージョン**として公開されていることを確認します。「[SharePoint Online で検索がすべての結果を返さない](https://go.microsoft.com/fwlink/?linkid=874525)」の手順 3 を実行します。</span><span class="sxs-lookup"><span data-stu-id="eee6a-p103">Verify that the page, document, or custom page layout is published as a **Major version.** Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="eee6a-p104">ユーザーがコンテンツを表示するための**アクセス許可**を持っていることを確認します。「[SharePoint でのアクセス許可レベルについて](https://docs.microsoft.com/sharepoint/understanding-permission-levels)」の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="eee6a-p104">Verify that the user has **permissions** to view the content. Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="eee6a-112">新しい管理プロパティの追加、管理プロパティの編集、または管理プロパティの削除により検索スキーマが変更されている場合は、その結果としてクロールおよびインデックスの再作成の要求が必須となります。</span><span class="sxs-lookup"><span data-stu-id="eee6a-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="eee6a-113">「[サイト、ライブラリ、またはリストのクロールおよびインデックスの再作成を手動で要求する](https://docs.microsoft.com/sharepoint/crawl-site-content)」の手順に従って、コンテンツの**インデックスの再作成**を行います。</span><span class="sxs-lookup"><span data-stu-id="eee6a-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="eee6a-114">これには時間を要します。結果を再度確認する前に24時間待ちます。</span><span class="sxs-lookup"><span data-stu-id="eee6a-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="eee6a-115">詳細については、[サイトのコンテンツを検索可能にする](https://docs.microsoft.com/sharepoint/make-site-content-searchable)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eee6a-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  

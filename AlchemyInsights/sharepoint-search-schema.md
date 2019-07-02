---
title: SharePoint Online の検索辞書を管理する
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 6c019de453a2185f42fa2fcffd8510fd06a33759
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35174462"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="c90dd-102">SharePoint Online で検索スキーマを管理する</span><span class="sxs-lookup"><span data-stu-id="c90dd-102">Manage the search schema in SharePoint Online</span></span>

<span data-ttu-id="c90dd-103">検索スキーマは、検索対象、検索方法、検索 Web サイトに検索結果を表示する方法を制御します。</span><span class="sxs-lookup"><span data-stu-id="c90dd-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="c90dd-104">検索スキーマを変更し、管理プロパティを作成し、クロールされたプロパティを管理プロパティにマップするには、「[SharePoint Online で検索スキーマを管理する](https://docs.microsoft.com/sharepoint/manage-search-schema)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c90dd-104">To change the search schema, create managed properties, and map crawled properties to managed properties, see [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema).</span></span> <span data-ttu-id="c90dd-105">スキーマ変更時に "アプリケーションは一時停止中です" という警告が表示される場合、これはサービスの保守が行われている間の一時的なものに過ぎません。</span><span class="sxs-lookup"><span data-stu-id="c90dd-105">If you receive a warning 'the application is paused' when making a schema change, this is only temporary there is service maintenance occurring.</span></span> 

<span data-ttu-id="c90dd-106">24 時間以上経過しても警告が表示される場合は、サポート ケースを記録してください。</span><span class="sxs-lookup"><span data-stu-id="c90dd-106">If more than 24 hours have passed and you're still experiencing the issue, please log a support ticket.</span></span>

<span data-ttu-id="c90dd-107">管理プロパティを変更するか、新しい管理プロパティを追加すると、その変更はコンテンツが再クロールされた後でのみ有効になります。</span><span class="sxs-lookup"><span data-stu-id="c90dd-107">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="c90dd-108">SharePoint Online では、定義されたクロール スケジュールに従って、クロールが自動的に行われます。</span><span class="sxs-lookup"><span data-stu-id="c90dd-108">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>

<span data-ttu-id="c90dd-109">変更が確実にクロールされるよう、[リストやライブラリのインデックスの再作成を具体的に要求](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)することができます。</span><span class="sxs-lookup"><span data-stu-id="c90dd-109">To make sure that your changes are crawled and reindexed, you can specifically request a reindexing of the list or library.</span></span> 

<span data-ttu-id="c90dd-110">検索スキーマの完全な概要については、「[Introducing Search Schema for SharePoint (SharePoint の検索スキーマの概要)](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c90dd-110">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


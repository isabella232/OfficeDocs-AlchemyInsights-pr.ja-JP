---
title: 1490 電子情報開示のエラーのトラブルシューティング
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277823"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="a3a56-102">コンテンツ検索のエラーをトラブルシューティングする</span><span class="sxs-lookup"><span data-stu-id="a3a56-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="a3a56-103">コンテンツ検索で問題が発生したり、検索結果をエクスポートする際にエラーを取得したりしている場合。</span><span class="sxs-lookup"><span data-stu-id="a3a56-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="a3a56-104">たとえば、検索の実行時に、次のようなことになる場合がありますか?</span><span class="sxs-lookup"><span data-stu-id="a3a56-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="a3a56-105">CS008 または CS012 エラー</span><span class="sxs-lookup"><span data-stu-id="a3a56-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="a3a56-106">サーバー ビジー/タイムアウト エラー</span><span class="sxs-lookup"><span data-stu-id="a3a56-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="a3a56-107">アプリケーション エラーが発生</span><span class="sxs-lookup"><span data-stu-id="a3a56-107">Application error occurred</span></span>

<span data-ttu-id="a3a56-108">または、多数のメールボックス (100,000 を超えるメールボックス) を検索したり、検索結果をエクスポートするときに、エクスポート エラーが発生しますか。</span><span class="sxs-lookup"><span data-stu-id="a3a56-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="a3a56-p101">このようなエラーの場合は、失敗したコンテンツの場所の検索を再試行してください。詳細については、[この記事](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3a56-p101">For these types of errors, retry the search for the content locations that have failed. See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="a3a56-111">10 万個以上のメールボックスをエクスポートする場合は、次の Powershell を使用し、エクスポート結果をダウンロードする必要があります: 「[10 万個以上のメールボックスから結果をエクスポートする](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)」。</span><span class="sxs-lookup"><span data-stu-id="a3a56-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>

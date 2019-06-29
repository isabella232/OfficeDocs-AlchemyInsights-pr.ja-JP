---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355882"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="3fdd8-102">期待した結果を返さないコンテンツ検索</span><span class="sxs-lookup"><span data-stu-id="3fdd8-102">Content Search not returning expected results</span></span>

<span data-ttu-id="3fdd8-p101">Office 365 セキュリティ/コンプライアンス センターからコンテンツ検索を実行すると、期待していない検索結果が返されることがあります。検索結果には、次の事項が影響している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3fdd8-p101">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results. Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="3fdd8-p102">**コンテンツの場所と検索条件**: 適切なコンテンツの場所と検索条件を選択していることを確認してください。大規模な検索 (多数の場所を含む) を実行する場合は、複数の検索に分割することを検討してください。</span><span class="sxs-lookup"><span data-stu-id="3fdd8-p102">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions. If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="3fdd8-p103">**部分的にインデックスが作成されたアイテム**: メールボックスから[部分的にインデックスが作成されたアイテム](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)は、推定される検索結果に含まれます。ただし、SharePoint および OneDrive のサイトからの部分的にインデックスが作成されたアイテムは検索の推定に含まれません。</span><span class="sxs-lookup"><span data-stu-id="3fdd8-p103">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results. However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="3fdd8-p104">**検索の失敗**: 多数のメールボックス (100,000 以上のメールボックス) を検索すると、CS008-009 や CS012-002 などのエラー コードと共にエラーが返されることがあります。この場合は、失敗したコンテンツの場所に対してのみ検索を再実行してみてください。詳細については、[この記事](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3fdd8-p104">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002). In this case, retry the search only for the failed content locations. See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>

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
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/22/2019
ms.locfileid: "31030744"
---
# <a name="content-search-not-returning-expected-results"></a>期待した結果を返さないコンテンツ検索

Office 365 セキュリティ/コンプライアンス センターからコンテンツ検索を実行すると、期待していない検索結果が返されることがあります。検索結果には、次の事項が影響している可能性があります。

- **コンテンツの場所と検索条件**: 適切なコンテンツの場所と検索条件を選択していることを確認してください。大規模な検索 (多数の場所を含む) を実行する場合は、複数の検索に分割することを検討してください。

- **部分的にインデックスが作成されたアイテム**: メールボックスから[部分的にインデックスが作成されたアイテム](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)は、推定される検索結果に含まれます。ただし、SharePoint および OneDrive のサイトからの部分的にインデックスが作成されたアイテムは検索の推定に含まれません。

- **検索の失敗**: 多数のメールボックス (100,000 以上のメールボックス) を検索すると、CS008-009 や CS012-002 などのエラー コードと共にエラーが返されることがあります。この場合は、失敗したコンテンツの場所に対してのみ検索を再実行してみてください。詳細については、[この記事](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)を参照してください。

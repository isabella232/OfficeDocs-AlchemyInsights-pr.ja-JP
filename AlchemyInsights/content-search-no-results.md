---
title: コンテンツ検索の結果がない
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816853"
---
# <a name="no-results-from-content-searchexports"></a>コンテンツ検索 / エクスポートの結果がない

コンテンツ検索 / エクスポートでデータが何も返されない問題は、特定の管理者によりセットアップされたものの、すべての管理者には伝達されなかった特定のコンプライアンス セキュリティ フィルターが原因の可能性があります。

この問題を解決するには、原因となっている可能性があるコンプライアンス セキュリティ フィルターがないかどうかを確認します。
1. セキュリティ/コンプライアンス センターの PowerShell に接続します。
2. 次のコマンドを実行します。
<br>$org = “yourdomain.com”
<br>Get-ComplianceSecurityFilter -Organization $org
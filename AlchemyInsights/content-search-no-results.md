---
title: コンテンツ検索の結果がない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516784"
---
# <a name="no-results-from-content-searchexports"></a>コンテンツ検索 / エクスポートの結果がない

コンテンツ検索 / エクスポートでデータが何も返されない問題は、特定の管理者によりセットアップされたものの、すべての管理者には伝達されなかった特定のコンプライアンス セキュリティ フィルターが原因の可能性があります。

この問題を解決するには、原因となっている可能性があるコンプライアンス セキュリティ フィルターがないかどうかを確認します。
1. セキュリティ/コンプライアンス センターの PowerShell に接続します。
2. 次のコマンドを実行します。
<br>$org = “yourdomain.com”
<br>Get-ComplianceSecurityFilter -Organization $org
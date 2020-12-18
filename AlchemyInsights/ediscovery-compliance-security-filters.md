---
title: コンテンツ検索/エクスポート中に結果が返されない
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680577"
---
# <a name="no-results-returned-during-content-searchexport"></a>コンテンツ検索/エクスポート中に結果が返されない

次の電子情報開示のシナリオで問題が発生している場合:

- コンテンツ検索/エクスポートは、データを返さないか、期待外のデータを返します。
- 電子情報開示の検索またはエクスポートが失敗する

特定の管理者によってセットアップされ、すべての管理者に通知されなかった特定のコンプライアンス セキュリティ フィルターが原因で、この問題が発生することがあります。

この問題を解決するには、原因となっている可能性があるコンプライアンス セキュリティ フィルターがないかどうかを確認します。

1. セキュリティ/コンプライアンス センターの PowerShell に接続します。
2. 次のコマンドを実行します。

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

コンプライアンス セキュリティ フィルターの詳細については、「[コンテンツ検索のアクセス許可フィルター](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)」を参照してください。

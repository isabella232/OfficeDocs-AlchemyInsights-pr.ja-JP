---
title: コンテンツ検索の結果がありません
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
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/19/2019
ms.locfileid: "35810582"
---
# <a name="no-results-from-content-searchexports"></a>コンテンツ検索/エクスポートからの結果がありません

コンテンツ検索/エクスポートに関する問題は、特定の管理者によってセットアップされた特定のコンプライアンスセキュリティフィルターによって、すべての管理者に伝達されないため、データが返されないことがあります。

この問題を解決するには、以下の原因と考えられるコンプライアンスセキュリティフィルターがあるかどうかを確認します。
1. セキュリティとコンプライアンスセンターの Powershell への接続
2. 次のコマンドレットを実行します。
<br>$org = "yourdomain.com"
<br>New-compliancesecurityfilter-組織 $org
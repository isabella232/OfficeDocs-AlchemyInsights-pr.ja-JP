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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516784"
---
# <a name="no-results-from-content-searchexports"></a>コンテンツ検索/エクスポートからの結果がありません

コンテンツ検索/エクスポートに関する問題は、特定の管理者によってセットアップされた特定のコンプライアンスセキュリティフィルターによって、すべての管理者に伝達されないため、データが返されないことがあります。

この問題を解決するには、以下の原因と考えられるコンプライアンスセキュリティフィルターがあるかどうかを確認します。
1. セキュリティとコンプライアンスセンターの Powershell への接続
2. 次のコマンドレットを実行します。
<br>$org = "yourdomain.com"
<br>New-compliancesecurityfilter-組織 $org
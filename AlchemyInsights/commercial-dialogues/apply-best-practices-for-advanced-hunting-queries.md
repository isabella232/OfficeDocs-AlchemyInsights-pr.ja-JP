---
title: 高度な捜索クエリのベスト プラクティスを適用する
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751336"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>高度な捜索クエリのベスト プラクティスを適用する

複雑なクエリを実行する際に、すばやく結果を取得してタイムアウトを回避するために、次のベスト プラクティスを適用してください。

- 新しいクエリを試行するときは、取得する結果セットが大きくなり過ぎないように、常に制限を使用します。 また、この `count` 使用して、結果セットのサイズを最初に評価します。
- 最初に時間フィルターを使用します。 クエリを 7 日に制限するのが理想です。
- クエリの最初、時間フィルターの使用直後に、ほとんどのデータを削除すると予想されるフィルターを追加します。
- 完全なトークンを探すときには、`contains` ではなく `has` 演算子を使用します。
- すべての列に対してではなく、特定の列で検索を実行します。
- テーブルを結合するときには、最初は行数が少ないテーブルを指定します。
- `project` は、結合したテーブルの必要な列に対してのみ使用します。

詳細については、「[高度な捜索クエリのベスト プラクティス](https://go.microsoft.com/fwlink/?linkid=2144812)」を参照してください。

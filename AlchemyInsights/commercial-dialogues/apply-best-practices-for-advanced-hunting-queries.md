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
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="f9cd3-102">高度な捜索クエリのベスト プラクティスを適用する</span><span class="sxs-lookup"><span data-stu-id="f9cd3-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="f9cd3-103">複雑なクエリを実行する際に、すばやく結果を取得してタイムアウトを回避するために、次のベスト プラクティスを適用してください。</span><span class="sxs-lookup"><span data-stu-id="f9cd3-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="f9cd3-104">新しいクエリを試行するときは、取得する結果セットが大きくなり過ぎないように、常に制限を使用します。</span><span class="sxs-lookup"><span data-stu-id="f9cd3-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="f9cd3-105">また、この `count` 使用して、結果セットのサイズを最初に評価します。</span><span class="sxs-lookup"><span data-stu-id="f9cd3-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="f9cd3-106">最初に時間フィルターを使用します。</span><span class="sxs-lookup"><span data-stu-id="f9cd3-106">Use time filters first.</span></span> <span data-ttu-id="f9cd3-107">クエリを 7 日に制限するのが理想です。</span><span class="sxs-lookup"><span data-stu-id="f9cd3-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="f9cd3-108">クエリの最初、時間フィルターの使用直後に、ほとんどのデータを削除すると予想されるフィルターを追加します。</span><span class="sxs-lookup"><span data-stu-id="f9cd3-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="f9cd3-109">完全なトークンを探すときには、`contains` ではなく `has` 演算子を使用します。</span><span class="sxs-lookup"><span data-stu-id="f9cd3-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="f9cd3-110">すべての列に対してではなく、特定の列で検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="f9cd3-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="f9cd3-111">テーブルを結合するときには、最初は行数が少ないテーブルを指定します。</span><span class="sxs-lookup"><span data-stu-id="f9cd3-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="f9cd3-112">`project` は、結合したテーブルの必要な列に対してのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="f9cd3-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="f9cd3-113">詳細については、「[高度な捜索クエリのベスト プラクティス](https://go.microsoft.com/fwlink/?linkid=2144812)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9cd3-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>

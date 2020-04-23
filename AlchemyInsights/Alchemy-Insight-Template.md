---
title: ファイル名と同じにするのが最適です
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676538"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="33d67-102">必要な Alchemy ヘッダー H1、H2 が機能していません。</span><span class="sxs-lookup"><span data-stu-id="33d67-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="33d67-103">Alchemy 作成のベスト プラクティスとガイドライン:</span><span class="sxs-lookup"><span data-stu-id="33d67-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="33d67-p101">**フォルダーで Alchemy 分析情報を入れ子にしないでください**- 入れ子にすると URL の構造が壊れてしまいます。この問題の修正については現在検討中です。</span><span class="sxs-lookup"><span data-stu-id="33d67-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="33d67-106">**AlchemyInsights** フォルダ内のファイルは、小文字のファイル名 (スペースの代わりにハイフンを使用) にする必要があります。例: </span><span class="sxs-lookup"><span data-stu-id="33d67-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="33d67-107">***how-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="33d67-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="33d67-108">[Alchemy パートナー ポータル](https://alchemyportal.azurewebsites.net)からのルール ID またはバケット ID を ms.custom フィールドに含めます。</span><span class="sxs-lookup"><span data-stu-id="33d67-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="33d67-109">例: </span><span class="sxs-lookup"><span data-stu-id="33d67-109">ex.</span></span> <span data-ttu-id="33d67-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="33d67-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="33d67-111">このファイルの冒頭にある残りのメタデータをテンプレートとして使用します。</span><span class="sxs-lookup"><span data-stu-id="33d67-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="33d67-112">[Alchemy Partner ポータル](https://alchemyportal.azurewebsites.net)で、セクション [**Customer Insight Title:**] まで下方向に移動し、それをインサイトの H1 タイトルの出発点として使用します。</span><span class="sxs-lookup"><span data-stu-id="33d67-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="33d67-p104">Alchemy Insight に含むことができる H1 は上部の 1 つに限られます。そうしなければ、運用環境では中断されます。H2 はレンダリングされないため、**太字**またはその他の規則を使用して、個別のセクションを表します。</span><span class="sxs-lookup"><span data-stu-id="33d67-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="33d67-115">次に、Alchemy Rule ページの Customer Insights セクションにある下書きの資料を使用して、本文のテキストを入力します。</span><span class="sxs-lookup"><span data-stu-id="33d67-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="33d67-116">箇条書きを使用できます。</span><span class="sxs-lookup"><span data-stu-id="33d67-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="33d67-117">段落番号も使用できます。</span><span class="sxs-lookup"><span data-stu-id="33d67-117">Numbered lists too</span></span>
    1. <span data-ttu-id="33d67-118">**太字**と*斜体*も使用できます。</span><span class="sxs-lookup"><span data-stu-id="33d67-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="33d67-119">リンクは常に、内部リンクではなく、**"Web へのリンク"/外部**または **UI 要素へのディープ リンク**のいずれかである必要があります。</span><span class="sxs-lookup"><span data-stu-id="33d67-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="33d67-120">現時点では画像は公式にはサポートされていませんが、ロードマップにあります。</span><span class="sxs-lookup"><span data-stu-id="33d67-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="33d67-121">実際には、これは少し長すぎます。</span><span class="sxs-lookup"><span data-stu-id="33d67-121">And this is really already a bit too long.</span></span> <span data-ttu-id="33d67-122">ベスト プラクティスは、約 400 文字です ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="33d67-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="33d67-123">コンテンツの準備ができたら、ライブ ブランチに抽出します。</span><span class="sxs-lookup"><span data-stu-id="33d67-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="33d67-124">次に、[Alchemy パートナー ポータル](https://alchemyportal.azurewebsites.net)に移動し、URL フィールドにファイル名を入力します。</span><span class="sxs-lookup"><span data-stu-id="33d67-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 
---
title: ファイル名と同じであることが最善 [ルール番号 - 説明]
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 01d8b03209e734f1218de61d964524b1b9e1d044
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939300"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="2425a-102">必要な Alchemy ヘッダー H1、H2 が機能していません。</span><span class="sxs-lookup"><span data-stu-id="2425a-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="2425a-103">Alchemy 作成のベスト プラクティスとガイドライン:</span><span class="sxs-lookup"><span data-stu-id="2425a-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="2425a-p101">**フォルダーで Alchemy 分析情報を入れ子にしないでください**- 入れ子にすると URL の構造が壊れてしまいます。この問題の修正については現在検討中です。</span><span class="sxs-lookup"><span data-stu-id="2425a-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="2425a-106">**AlchemyInsights** フォルダー内のファイルには、ファイル名に [Alchemy Partner ポータル](https://alchemyportal.azurewebsites.net)のルール ID とルール名が含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2425a-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="2425a-p102">例: ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="2425a-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="2425a-p103">このファイルの冒頭にあるメタデータをテンプレートとして使用します。それ以外のものは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="2425a-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="2425a-111">[Alchemy Partner ポータル](https://alchemyportal.azurewebsites.net)で、セクション [**Customer Insight Title:**] まで下方向に移動し、それをインサイトの H1 タイトルの出発点として使用します。</span><span class="sxs-lookup"><span data-stu-id="2425a-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="2425a-p104">Alchemy Insight に含むことができる H1 は上部の 1 つに限られます。そうしなければ、運用環境では中断されます。H2 はレンダリングされないため、**太字**またはその他の規則を使用して、個別のセクションを表します。</span><span class="sxs-lookup"><span data-stu-id="2425a-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="2425a-114">次に、Alchemy Rule ページの Customer Insights セクションにある下書きの資料を使用して、本文のテキストを入力します。</span><span class="sxs-lookup"><span data-stu-id="2425a-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="2425a-115">箇条書きを使用できます。</span><span class="sxs-lookup"><span data-stu-id="2425a-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="2425a-116">段落番号も使用できます。</span><span class="sxs-lookup"><span data-stu-id="2425a-116">Numbered lists too</span></span>
    1. <span data-ttu-id="2425a-117">**太字**と*斜体*も使用できます。</span><span class="sxs-lookup"><span data-stu-id="2425a-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="2425a-118">リンクは常に、内部リンクではなく、**"Web へのリンク"/外部**または **UI 要素へのディープ リンク**のいずれかである必要があります。</span><span class="sxs-lookup"><span data-stu-id="2425a-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="2425a-p105">また、これは実際には既に少し長すぎます。ベスト プラクティスは約 400 文字です ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="2425a-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="2425a-p106">コンテンツの準備ができたら、ライブ ブランチに抽出します。次に、[Alchemy Partner ポータル](https://alchemyportal.azurewebsites.net)に移動して、ファイル名を URL フィールドに入力します。確認および発行された分析情報に "はい" と示されていることを確認し、[ルールの更新] をクリックします **(間もなくリリースされる新しいバージョンのポータルではより見栄えが良くなっています)。**
![URL フィールド](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="2425a-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>


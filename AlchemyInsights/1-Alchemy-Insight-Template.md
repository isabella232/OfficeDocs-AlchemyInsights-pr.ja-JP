---
title: ファイル名と同じであることが最善 [ルール番号 - 説明]
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 9e2a369f4b1bf87da8b12224b5f6e8b1138db9dd
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29454219"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a><span data-ttu-id="ef1ef-102">必須の顧客に接続する H1、H2 は機能しません。</span><span class="sxs-lookup"><span data-stu-id="ef1ef-102">Required Customer Facing H1, H2 doesn't work</span></span>
<span data-ttu-id="ef1ef-103">テキスト ブロックの例 - 次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="ef1ef-103">Example text block - follow these instructions:</span></span>

1. <span data-ttu-id="ef1ef-104">**AlchemyInsights** フォルダー内のファイルには、[Alchemy Partner ポータル](https://alchemyportal.azurewebsites.net)のルール ID とルール名が含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef1ef-104">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the mane.</span></span>
    1. <span data-ttu-id="ef1ef-p101">例: ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="ef1ef-p101">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="ef1ef-p102">このファイルの冒頭にあるメタデータをテンプレートとして使用します。それ以外のものは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="ef1ef-p102">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="ef1ef-109">[Alchemy Partner ポータル](https://alchemyportal.azurewebsites.net)で、セクション [**Customer Insight Title:**] まで下方向に移動し、それをインサイトの H1 タイトルの出発点として使用します。</span><span class="sxs-lookup"><span data-stu-id="ef1ef-109">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="ef1ef-p103">Alchemy Insight に含むことができる H1 は上部の 1 つに限られます。そうしなければ、運用環境では中断されます。H2 はレンダリングされないため、**太字**またはその他の規則を使用して、個別のセクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ef1ef-p103">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="ef1ef-112">次に、Alchemy Rule ページの Customer Insights セクションにある下書きの資料を使用して、本文のテキストを入力します。</span><span class="sxs-lookup"><span data-stu-id="ef1ef-112">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="ef1ef-113">箇条書きを使用できます。</span><span class="sxs-lookup"><span data-stu-id="ef1ef-113">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="ef1ef-114">段落番号も使用できます。</span><span class="sxs-lookup"><span data-stu-id="ef1ef-114">Numbered lists too</span></span>
    1. <span data-ttu-id="ef1ef-115">**太字**と*斜体*も使用できます。</span><span class="sxs-lookup"><span data-stu-id="ef1ef-115">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="ef1ef-116">リンクは常に、内部リンクではなく、**"Web へのリンク"/外部**または **UI 要素へのディープ リンク**のいずれかである必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef1ef-116">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="ef1ef-p104">また、これは実際には既に多少長すぎます。ベスト プラクティスは約 400 文字です ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="ef1ef-p104">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>
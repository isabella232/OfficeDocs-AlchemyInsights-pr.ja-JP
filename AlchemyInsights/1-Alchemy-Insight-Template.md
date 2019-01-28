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
# <a name="required-customer-facing-h1-h2-doesnt-work"></a>必須の顧客に接続する H1、H2 は機能しません。
テキスト ブロックの例 - 次の手順に従います。

1. **AlchemyInsights** フォルダー内のファイルには、[Alchemy Partner ポータル](https://alchemyportal.azurewebsites.net)のルール ID とルール名が含まれている必要があります。
    1. 例: ***976-How-to-enable-litigation-hold***
1. このファイルの冒頭にあるメタデータをテンプレートとして使用します。それ以外のものは必要ありません。
1. [Alchemy Partner ポータル](https://alchemyportal.azurewebsites.net)で、セクション [**Customer Insight Title:**] まで下方向に移動し、それをインサイトの H1 タイトルの出発点として使用します。 
    > [!NOTE]
    > Alchemy Insight に含むことができる H1 は上部の 1 つに限られます。そうしなければ、運用環境では中断されます。H2 はレンダリングされないため、**太字**またはその他の規則を使用して、個別のセクションを表します。
1. 次に、Alchemy Rule ページの Customer Insights セクションにある下書きの資料を使用して、本文のテキストを入力します。
    1. 箇条書きを使用できます。
    1. 段落番号も使用できます。
    1. **太字**と*斜体*も使用できます。
    1. リンクは常に、内部リンクではなく、**"Web へのリンク"/外部**または **UI 要素へのディープ リンク**のいずれかである必要があります。

また、これは実際には既に多少長すぎます。ベスト プラクティスは約 400 文字です ---------------------------------
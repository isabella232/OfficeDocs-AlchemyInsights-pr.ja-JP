---
title: ファイル名と同じにするのが最適です
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312830"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"必要な Alchemy ヘッダー H1、H2 が機能していません。"
Alchemy 作成のベスト プラクティスとガイドライン:

1. **フォルダーで Alchemy 分析情報を入れ子にしないでください**- 入れ子にすると URL の構造が壊れてしまいます。この問題の修正については現在検討中です。
1. **AlchemyInsights** フォルダ内のファイルは、小文字のファイル名 (スペースの代わりにハイフンを使用) にする必要があります。例: **_how-to-enable-litigation-hold_**。
    1. [Alchemy パートナー ポータル](https://alchemyportal.azurewebsites.net)からのルール ID またはバケット ID を ms.custom フィールドに含めます。例: ***ms.custom: 100021***
1. このファイルの冒頭にある残りのメタデータをテンプレートとして使用します。
1. [Alchemy Partner ポータル](https://alchemyportal.azurewebsites.net)で、セクション [**Customer Insight Title:**] まで下方向に移動し、それをインサイトの H1 タイトルの出発点として使用します。 

**注**: Alchemy Insight に含むことができる H1 は上部の 1 つに限られます。そうしなければ、運用環境では中断されます。H2 はレンダリングされないため、**太字** またはその他の規則を使用して、個別のセクションを表します。
1. 次に、Alchemy Rule ページの Customer Insights セクションにある下書きの資料を使用して、本文のテキストを入力します。
    1. 箇条書きを使用できます。
    1. 段落番号も使用できます。
    1. **太字** と *斜体* も使用できます。
    1. リンクは常に、内部リンクではなく、**"Web へのリンク"/外部** または **UI 要素へのディープ リンク** のいずれかである必要があります。
    1. 現時点では画像は公式にはサポートされていませんが、ロードマップにあります。

また、これは実際には既に少し長すぎます。ベスト プラクティスは約 400 文字です ---------------------------------

コンテンツの準備ができたら、ライブ ブランチに抽出します。次に、[Alchemy Partner ポータル](https://alchemyportal.azurewebsites.net)に移動して、ファイル名を URL フィールドに入力します。 
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
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750975"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"必要な Alchemy ヘッダー H1、H2 が機能していません。"
Alchemy 作成のベスト プラクティスとガイドライン:

1. **Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.
1. **AlchemyInsights** フォルダ内のファイルは、小文字のファイル名 (スペースの代わりにハイフンを使用) にする必要があります。例:  ***how-to-enable-litigation-hold***
    1. [Alchemy パートナー ポータル](https://alchemyportal.azurewebsites.net)からのルール ID またはバケット ID を ms.custom フィールドに含めます。 例:  ***ms.custom: 100021***
1. このファイルの冒頭にある残りのメタデータをテンプレートとして使用します。
1. [Alchemy Partner ポータル](https://alchemyportal.azurewebsites.net)で、セクション [**Customer Insight Title:**] まで下方向に移動し、それをインサイトの H1 タイトルの出発点として使用します。 
    > [!NOTE]
    > Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.
1. 次に、Alchemy Rule ページの Customer Insights セクションにある下書きの資料を使用して、本文のテキストを入力します。
    1. 箇条書きを使用できます。
    1. 段落番号も使用できます。
    1. **太字**と*斜体*も使用できます。
    1. リンクは常に、内部リンクではなく、**"Web へのリンク"/外部**または **UI 要素へのディープ リンク**のいずれかである必要があります。
    1. 現時点では画像は公式にはサポートされていませんが、ロードマップにあります。

実際には、これは少し長すぎます。 ベスト プラクティスは、約 400 文字です ---------------------------------

コンテンツの準備ができたら、ライブ ブランチに抽出します。 次に、[Alchemy パートナー ポータル](https://alchemyportal.azurewebsites.net)に移動し、URL フィールドにファイル名を入力します。 
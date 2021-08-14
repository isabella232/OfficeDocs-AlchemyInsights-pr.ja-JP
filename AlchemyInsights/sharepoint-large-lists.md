---
title: SharePoint の大きなリスト
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: c67632e323f2068faba06779b94ba4fd8e9f319e18cefb7977bd3038ca770210
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53941608"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>SharePoint で大きなリストおよびライブラリを使用する

SharePoint のリストおよびライブラリには、最大 3,000 万個のアイテムを含めることができます。ただし、5,000 個を超えるアイテムが含まれる場合、それらを使用しようとすると、リスト ビューのしきい値エラーが表示されることがあります。このしきい値は、サービスのパフォーマンスを維持するために設定されており、変更することはできません。このしきい値に達しないようにするには、次を実行します。

**モダンを使用する**

表示アイテムが多いビューの場合、モダン環境で最適に動作します。 [モダン環境を使用](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9)すると、クラシック環境で発生する可能性があるエラーを回避できます。

**インデックスを追加する**

インデックスが作成されていない列によるフィルター処理または並べ替えを実行すると、エラー メッセージが表示される場合があります。 [設定] メニューの [**リストの設定**] から手動で [インデックスを追加](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0)してから、**インデックス付きの列** を追加します。

**リスト ビューを編集する**

大規模なリストでの作業でエラーが発生する場合は、[リスト ビューを編集します](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)。

次の 4 つの変更により、リスト ビューのしきい値エラーが削除されます。 4 つの変更をすべて行って、すべてのエラーを削除します。 それでもエラーが発生する場合は、「[大規模なリストとライブラリ](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)」を確認してください。

1. [**最優先する列**] と [**2 番目に優先する列**] の両方から [**なし**] を選択します。
2. [**最優先する列**] と [**2 番目に優先する列**] の両方から [**なし**] を選択します。
3. [**合計**] セクションのすべての列で [**なし**] を選択します。
4. [**列**] セクションから表示する 1 列を除くすべての選択を解除します。


---
title: グリッド内のさまざまなレコード数を示すグラフ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 68ba6caf602a5cf60e2c96c80703f19dd07c3b6430c2a66f40fea4a2f3d06e75
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950085"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>グリッド内のさまざまなレコード数を示すグラフ

**現象**

ダッシュボードページのグラフに、グラフ"..."をクリックし、[レコードを表示]グリッドをクリックすると、ページに移動してすべてのレコードを表示することができます。レコードの数が変わることがあります。

**原因**

これは、元のダッシュボードページ上のグラフとグリッドのホームページのグラフのビューの違いが原因です。  

**解決方法**

1. 元のページとグリッドのビューを見て、それらが異なるかどうかを確認します。
2. 元のページのビューと一致するようにグリッドのビューを変更します。
3. 正しいビューが見つからない場合は、通常、アプリデザイナーでビューが有効になっていないことを意味します。
4. 特定のアプリのアプリデザイナーに移動して、エンティティとビューを選択し、変更を希望するビューで有効、保存、発行にチェックを入れてから閉じます。
5. ページを更新します。
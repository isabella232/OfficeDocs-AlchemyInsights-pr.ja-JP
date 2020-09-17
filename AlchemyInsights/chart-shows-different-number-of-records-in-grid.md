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
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793763"
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
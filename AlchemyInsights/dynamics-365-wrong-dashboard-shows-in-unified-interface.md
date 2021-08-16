---
title: Dynamics 365 - Dynamics 365 統合インターフェイスでの間違ったダッシュボードの表示
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101487"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 統合インターフェースで間違ったダッシュボードが表示される

想定と異なるダッシュボードが表示される理由はいくつかあります。

## <a name="the-user-has-set-a-user-default-dashboard"></a>ユーザーが自分のデフォルトのダッシュボードを設定した 

通常、[**デフォルトに設定**] ボタンがダッシュボードのコマンド バーに表示されない場合は、ユーザーのデフォルト ダッシュボードが設定されていると認識できます。 ユーザーのデフォルト ダッシュボードが現在のアプリに含まれていない場合でも、ユーザーのデフォルト ダッシュボードは他のすべてのデフォルトのダッシュボードを上書きします。

デフォルトのダッシュボードの設定を解除するには、次の回避策を使用してください。

1. 新しい個人用ダッシュボードを作成します。

2. 新しいダッシュボードをユーザーのデフォルトとして設定します。

3. そのダッシュボードを削除します。

## <a name="the-dashboard-is-set-in-the-sitemap"></a>ダッシュボードがサイトマップに設定されている

ダッシュボードを選択し、 [システムのカスタマイズ] の下にある [デフォルトに設定] を選んで、組織のデフォルト ダッシュボードを設定したでしょうか。 ですが、ユーザーがアクセス権を持っている場合、サイトマップデザイナーで定義されているダッシュボードがこのダッシュボードよりも優先されます。

組織のデフォルトとして設定したダッシュボードをユーザーに表示させるには、次のいずれかの操作を行います。

* そのダッシュボードをサイトマップに設定する

* それらのユーザーのサイトマップ定義ダッシュボードへのアクセス権を削除する

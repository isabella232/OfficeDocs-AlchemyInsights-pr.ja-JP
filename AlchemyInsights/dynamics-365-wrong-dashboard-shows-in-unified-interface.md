---
title: Dynamics 365-Dynamics 365 の統合インターフェイスに正しくないダッシュボードが表示される
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528556"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 の統合インターフェイスに正しくないダッシュボードが表示される

必要なダッシュボードとは異なるダッシュボードが表示される理由はいくつかあります。

## <a name="the-user-has-set-a-user-default-dashboard"></a>ユーザーがユーザーの既定のダッシュボードを設定した 

通常、ユーザーの既定のダッシュボードは、[既定の**設定**] ボタンがダッシュボードのコマンドバーに表示されない場合に設定できます。 ユーザーの既定のダッシュボードが現在のアプリにない場合でも、ユーザーの既定のダッシュボードは他のすべての既定のダッシュボードを上書きします。

次の回避策を使用して、既定のダッシュボードを未設定にします。

1. 新しい個人ダッシュボードを作成します。

2. 新しいダッシュボードをユーザーの既定として設定します。

3. そのダッシュボードを削除します。

## <a name="the-dashboard-is-set-in-the-sitemap"></a>ダッシュボードは sitemap で設定されています。

ダッシュボードを選択し、[システムのカスタマイズ] の [既定として設定] を選択することにより、組織の既定のダッシュボードを設定した可能性があります。 しかし、ユーザーがアクセス権を持っている場合は、sitemap designer で定義されたダッシュボードがこのダッシュボードより優先されます。

組織の既定値として設定したダッシュボードがユーザーに表示されるようにするには、次のいずれかの方法を使用できます。

* Sitemap でそのダッシュボードを設定する

* これらのユーザーの sitemap 定義済みダッシュボードへのアクセスを削除する

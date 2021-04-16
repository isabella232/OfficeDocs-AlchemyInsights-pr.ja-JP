---
title: Windows 10 で電源アイコンまたはバッテリー アイコンが表示されない
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790553"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Windows 10 で電源アイコンまたはバッテリー アイコンが表示されない

Windows 10 デバイスにバッテリーが搭載されている場合 (たとえば、ノート PC またはタブレット、または USB 経由で UPS に接続された PC)、通常、電源/バッテリー アイコンが時計の近くのタスクバーに表示されます。次に例を示します。

![バッテリー アイコン](media/battery-icon.png)

このアイコンが表示されない場合は、非表示になっている可能性があります。

1. **[[設定]、[個人用設定]、[タスクバー]](ms-settings:taskbar?activationSource=GetHelp)** の順に移動します。

2. 通知領域で [**タスク バーに表示するアイコンの選択**] をクリックします。

3. 次に、リストから [**電源**] アイテムを見つけ、その設定を [**オン**] に切り替えます。

    ![タスクバーに電源アイコンを表示する](media/power-icon-on.png)

**トラブルシューティング**

上記の手順に従っても、[**電源**] トグルが灰色表示されている、または表示されない場合は、タスクバーの検索ボックスに「**デバイス マネージャー**」と入力し、入力結果のリストから [**デバイス マネージャー**] を選択します。 [**バッテリー**] で、デバイスのバッテリーを右クリックし、[**無効にする**] をクリックして、[**はい**] をクリックします。 数秒待ってからバッテリーを右クリックし、[**有効にする**] をクリックします。 デバイスを再起動します。

上記の手順に従っても、バッテリー アイコンがタスクバーに表示されない場合は、タスクバーの検索ボックスに「**デバイス マネージャー**」と入力し、入力結果のリストから [**デバイス マネージャー**] を選択します。 [**プロセス**] タブの [**名前**] で、[**エクスプローラー**] を右クリックし、[**再起動**] をクリックします。

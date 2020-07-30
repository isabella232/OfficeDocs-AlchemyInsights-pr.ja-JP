---
title: Intune からのデータの削除とデバイスのワイプ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440609"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Intune からのデータの削除とデバイスのワイプ

Device Retire およびDevice Wipe リモートアクションを使用して、Intune が管理する会社データを削除したり、デバイスを出荷時設定にリセットして既定の設定に戻すことができます。

1. Microsoft 365 Device Management にサインインし、**デバイス**の > **すべてのデバイス**に移動します。
2. ワイプを実行するデバイスを選びます。
3. 実行するリモートワイプのタイプを選択します。 破棄を行うと組織情報のみが削除されますが、フルワイプを実行すると、デバイスは工場出荷時の設定に戻ります。
4. [**はい**] を選択して確認します。 ワイプが完了するまで、デバイスのアクションステータスは [破棄の保留中] と表示されます。</br>
    アクションが完了すると、管理対象デバイスのリストにモバイルデバイスが表示されなくなります。

**注:** 会社のデータを Azure AD に結合されたデバイスから削除することはできません。

何が保持され何が削除されるかなど、破棄およびワイプ アクションの効果の詳細については、「[ワイプを使用してデバイスを削除、破棄、または手動でデバイスの登録を解除する](https://docs.microsoft.com/intune/devices-wipe)」を参照してください。

MacOS デバイスのすべてのデータを消去する場合は、「[MacOS デバイスからすべてのデータを削除する](https://docs.microsoft.com/intune/device-erase)」を参照してください。
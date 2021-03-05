---
title: Intune からのデータの削除とデバイスのワイプ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416318"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Intune からのデータの削除とデバイスのワイプ

Device Retire およびDevice Wipe リモートアクションを使用して、Intune が管理する会社データを削除したり、デバイスを出荷時設定にリセットして既定の設定に戻すことができます。

1. Microsoft 365 Device Management にサインインし、**デバイス** の > **すべてのデバイス** に移動します。
2. ワイプを実行するデバイスを選びます。
3. 実行するリモートワイプのタイプを選択します。 破棄を行うと組織情報のみが削除されますが、フルワイプを実行すると、デバイスは工場出荷時の設定に戻ります。
4. [**はい**] を選択して確認します。 ワイプが完了するまで、デバイスのアクションステータスは *[破棄の保留中]* と表示されます。
    アクションが完了すると、管理対象デバイスのリストにモバイルデバイスが表示されなくなります。

> [!NOTE]
> 会社のデータを Azure AD に結合されたデバイスから削除することはできません。 

何が保持され何が削除されるかなど、破棄およびワイプ アクションの効果の詳細については、以下のドキュメントを参照してください。

- [ワイプ、インベントリからの削除、デバイス登録の手動解除を使用し、デバイスを削除する](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)。
- [Intune で管理されているアプリから会社のデータをワイプする方法](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [MacOS デバイスからすべてのデータを削除する](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)。
---
title: Intune を使用して、管理している iOS デバイスのアクティベーション ロックをバイパスする
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424325"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Intune を使用して、管理している iOS デバイスのアクティベーション ロックをバイパスする

iOS デバイスのアクティベーション ロックをバイパスする機能を利用すると、ユーザーが会社のデバイスでアクティベーション ロックを有効にして会社を去るシナリオからの回復が容易になります。

アクティベーション ロックをバイパスするための前提条件:

- 「監視」されているデバイスです。
- Intune での iOS デバイス制限ポリシーを使用して、アクティベーション ロックが正常に有効になります。

また、アクティベーション ロックをバイパスする場合は、次の操作を行う必要があります:

- ワイプされるデバイスを物理的に所有します。
- ワイプを実行する前に、コードをコピーします。

**注:** ワイプ コードの大文字と小文字は区別されないため、「-」文字は必要ありません。

詳細については、[「Intune を使用して、管理している iOS デバイスのアクティベーション ロックをバイパスする」](https://docs.microsoft.com/intune/device-activation-lock-bypass) を参照してください。

**FAQ**

Q: **デバイスから会社のデータを削除するためのリモート アクションを発行したところ、保留状態のままになっています。**

A: リモートアクションを正常に完了するには、対象のデバイスがオンラインで正常である必要があります。 次のような状況では、リモート アクションは、30 日間、またはデバイスの場合デバイスがコマンドを認識するまで、保留状態になります:

- 接続がありません。
- Intune で管理状態が失われています。

デバイスがチェックされず、会社のデータが削除されない場合は、[削除] を選択します。 削除すると、デバイスのレコードが削除され、デバイスの Intune リストに表示されなくなります。 デバイスをもう一度アクティブにするには、デバイスを再登録する必要があります。

Q: **特定のリモート アクションを使用できないのはなぜですか?**

A: すべてのプラットフォームがすべてのリモート デバイス アクションをサポートしているわけではありません。 次のリモート アクションはプラットフォーム固有です。

- アクティベーション ロックのバイパス (iOS のみ)
- 新たに開始 (Windows のみ)
- ロスト モード (iOS のみ)
- デバイスの検索 (iOS のみ)
- 再起動 (Windows のみ)

各アクションの詳細については、[「使用可能なデバイス アクション」](https://docs.microsoft.com/intune/device-management#available-device-actions) を参照してください。
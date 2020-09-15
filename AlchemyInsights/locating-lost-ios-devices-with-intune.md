---
title: 紛失した iOS デバイスを Intune で見つける
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
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675171"
---
# <a name="locating-lost-ios-devices-with-intune"></a>紛失した iOS デバイスを Intune で見つける

iOS デバイスで紛失モードを有効にすると、管理者はロック画面にメッセージと連絡先の電話番号を表示できます。

紛失モードを有効にした後、管理者は [デバイスの検索] アクションを使用して、デバイスの物理的な場所を特定できます。

Intuneのデバイス検索アクションは iOS デバイス上で、特定のデバイスの場所を地図上に表示します。

このアクションを使用するには、iOS デバイスが次のいずれかの状態である必要があります。

- 監視モード
- 紛失モード

詳細については、[「 Intune で iOS / iPadOS デバイスで紛失モードを有効にする」](https://docs.microsoft.com/intune/device-lost-mode)および[「Intuneで紛失または盗難された iOS / iPadOS デバイスを特定する」](https://docs.microsoft.com/intune/device-locate)を参照してください。

**FAQ**

Q：会社のデータをデバイスから削除するためのリモート アクションを発行しましたが、保留状態のままになっています。

A: リモート アクションを正常に完了するには、対象のデバイスがオンラインで正常である必要があります。 次のような状況では、リモート アクションは30日間、またはデバイスがコマンドを確認するまで保留状態になります。

- デバイスが接続できない場合
- デバイスで Intune の管理状態が解除された場合

デバイスがチェックインしておらず、会社のデータを削除できない場合は、[削除]を選択します。 削除すると、デバイスのレコードが削除され、デバイスの Intune リストに表示されなくなります。 デバイスが再びアクティブになった場合、そのユーザーはデバイスを再登録する必要があります。

Q: 特定のリモート アクションを使用できないのはなぜですか?

A: すべてのプラットフォームがすべてのリモート デバイス アクションをサポートしているわけではありません。 以下のリモートアクションはプラットフォーム固有であるため、記載されているプラットフォームでのみ使用できます。

- アクティベーション ロックのバイパス (iOS のみ)
- 新たに開始 (Windows のみ)
- ロスト モード (iOS のみ)
- デバイスの検索 (iOS のみ)
- 再起動 (Windows のみ)

各アクションの詳細については、[「使用可能なデバイス アクション」](https://docs.microsoft.com/intune/device-management#available-device-actions) を参照してください。
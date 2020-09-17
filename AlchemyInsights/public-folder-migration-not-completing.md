---
title: パブリック フォルダーの移行バッチが完了せず、同期が表示される
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 33302110249b02aef87639792ebfd9cafd6638c0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47804427"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a>パブリック フォルダーの移行バッチが完了せず、同期が表示される

移行バッチの完了を開始した可能性があり、移行バッチの状態が非常に長い間 [同期済み] と表示され続けます。 これは想定された動作です。

移行バッチの状態は、[完了] に切り替わる前に数時間 [同期済み] のままになるのが一般的です。 多数のターゲット メールボックスを含む移行の場合、基になるパブリック フォルダーの移行の要求が失敗または検疫されていない限り、状態は 24 時間以上 [同期済み] 状態のままです。 移行バッチがタスクを完了するまでに 24 - 48 時間かかります。

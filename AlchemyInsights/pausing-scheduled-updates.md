---
title: スケジュール済みの更新の一時停止
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2020
ms.locfileid: "46556250"
---
# <a name="pausing-scheduled-updates"></a>スケジュール済みの更新の一時停止

[一時停止] コマンドが発行されると、デバイスは次回 Intune にチェックインするまでコマンドを処理しません。 このため、デバイスは次のことを行う、または状態にある可能性があります:

- チェックイン前にスケジュール済みの更新をインストールしている。
- [一時停止] コマンドを発行したときに電源がオフになる。 この場合、デバイスの電源を入れたときに、チェックイン前からスケジュール済みの更新をダウンロードしてインストールした可能性があります。
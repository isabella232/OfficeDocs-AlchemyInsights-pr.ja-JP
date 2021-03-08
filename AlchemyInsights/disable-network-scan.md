---
title: ネットワーク スキャンを無効にする
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50484074"
---
# <a name="disable-network-scan"></a>ネットワーク スキャンを無効にする

ネットワーク共有スキャンはパフォーマンスに影響を与える可能性があります。  クライアントがデフォルトでネットワーク共有 / ファイルをスキャンしないようにするには、Windows Defender アプリケーションで次の設定を **True** に構成します。

- DisableScanningMappedNetworkDrivesForFullScan
- DisableScanningNetworkFiles
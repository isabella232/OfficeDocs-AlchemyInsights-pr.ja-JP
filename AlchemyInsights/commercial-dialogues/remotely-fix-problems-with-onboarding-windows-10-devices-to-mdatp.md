---
title: Windows 10 デバイスの Microsoft Defender Advanced Threat Protection へのオンボーディングに関する問題をリモートで修正する
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034039"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Windows 10 デバイスの Microsoft Defender Advanced Threat Protection へのオンボーディングに関する問題をリモートで修正する

リモート コンピューターにアクセスできる場合は、次の手順を実行します。

1. [クライアント接続アナライザー](https://go.microsoft.com/fwlink/?linkid=2143466)の診断ツールをダウンロードします。
2. 展開し、MDATPAnalyzer.cmd を実行します。
3. MDATPClientAnalyzerResult フォルダーにある診断ログを見つけます。これは、アナライザー ツールがダウンロードされたフォルダーと同じです。
4. ログ ファイル MDATPClientAnalyzer.txt を確認して、接続またはインターネット プロキシ設定に関する問題を見つけます。

詳細については、「[マシンのオンボードの問題](https://go.microsoft.com/fwlink/?linkid=2143634)」を参照してください。

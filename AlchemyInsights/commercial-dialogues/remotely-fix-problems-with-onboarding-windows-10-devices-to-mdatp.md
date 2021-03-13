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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751374"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Windows 10 デバイスの Microsoft Defender Advanced Threat Protection へのオンボーディングに関する問題をリモートで修正する

リモート コンピューターにアクセスできる場合は、次の手順を実行します。

1. [クライアント接続アナライザー](https://go.microsoft.com/fwlink/?linkid=2143466)の診断ツールをダウンロードします。
2. 展開し、MDATPAnalyzer.cmd を実行します。
3. MDATPClientAnalyzerResult フォルダーにある診断ログを見つけます。これは、アナライザー ツールがダウンロードされたフォルダーと同じです。
4. ログ ファイル MDATPClientAnalyzer.txt を確認して、接続またはインターネット プロキシ設定に関する問題を見つけます。

詳細については、「[マシンのオンボードの問題](https://go.microsoft.com/fwlink/?linkid=2143634)」を参照してください。

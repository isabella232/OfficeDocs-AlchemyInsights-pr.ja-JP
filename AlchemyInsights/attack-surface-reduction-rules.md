---
title: 攻撃面の減少ルール
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 0f2e3d2d2cfa205f95a5d5dc84f7293fbee165a2976248de75a96379becd6925
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072201"
---
# <a name="attack-surface-reduction-rules"></a>攻撃面の減少ルール

ファイルやフォルダーを除外すると、攻撃面の減少ルールで指定された保護機能が著しく低下します。 ルールでブロックされたはずのファイルは実行が許可され、レポートやイベントは記録されません。 除外は、除外を許可するすべてのルールに適用されます。

ASR の除外項目は、Microsoft Defender ウイルス対策の除外項目と同じ構文を使用します。 詳細については、「[Windows Defender ウイルス対策のスキャンの除外項目の構成と検証](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)」を参照してください。 問題を回避するには、「[除外を定義する際に避ける必要のある一般的な間違い](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)」を確認してください。

すべての ASR ルールが除外項目をサポートしているわけではありません。 ルールが除外項目をサポートしているかどうかを検証するには、テーブル「[攻撃面の減少ルール](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)」を参照してください。

## <a name="attack-surface-reduction-rules"></a>攻撃面の減少ルール

組織の攻撃面とは、攻撃者が組織のデバイスやネットワークを侵害する可能性のあるすべての場所を指します。 攻撃対象を削減するということは、組織のデバイスやネットワークを保護し、攻撃者が攻撃を実行する手段を減らすことを意味します。 Microsoft Defender for Endpoint で攻撃面の減少ルールを構成することが役立ちます。

詳細については、以下を参照してください。

- [ASR ルール GUID をマッピングして名前をつける](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- ASR ルールの要件は、以下のとおりです。
    - [Windows 10 バージョン 1709 以降](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise バージョン 1709 以降](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server バージョン 1803 (半期チャネル) 以降](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>適用する適切な除外項目を特定する

1. Microsoft - Windows - Windows Defender/Operational のログで eventID 1121 または 1122 であることを確認します。

1. ブロック シナリオとコンテキストを評価し、このシナリオはブロックを解除する必要があることを確認します。

1. イベントの詳細にある、除外を定義する値である Path の値を読み取ります。
    - 除外項目はできるだけ厳密にしてください。
    - 必要に応じてワイルドカードを適用します (User 変数の置き換えなど)。

1. 展開の必要性に応じて、除外事項を適用します。 詳細については、「[攻撃面の減少ルールをカスタマイズする](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)」を参照してください。

## <a name="exclusion-is-not-honored"></a>除外事項が受け入れられない

1. ルールが除外事項をサポートしているかどうか判断します。 詳細については、「[攻撃面の減少ルール](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)」を参照してください。

1. 適用された除外項目を確認し、タイプミスや誤って解釈されたワイルドカードがないか、イベント データで検証します。 詳細については、「[サポートされる除外タイプ](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)」を参照してください

1. ルールの影響が大きすぎる場合は、ルールを監査モードに戻してさらに検証を行うことを検討します。 詳細については、「[Microsoft Defender for Endpoint 機能が監査モードで動作する方法を確認する](/microsoft-365/security/defender-endpoint/audit-windows-defender)」を参照してください。

1. このコマンドを使用してサポート ケースを開くためのサポートデータを収集します。
    
   ** MDEClientAnalyzer.cmd -v**

    詳細については、「[Microsoft Defender for Endpoints へのマシンのオンボードに関する問題](issues-with-onboarding-machines.md)」を参照してください。

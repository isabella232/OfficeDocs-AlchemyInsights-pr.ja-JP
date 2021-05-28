---
title: Defender Endpoint でセンサーの状態をチェックする
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676598"
---
# <a name="defender-endpoint-check-sensor-status"></a>Defender Endpoint でセンサーの状態をチェックする

**センサーに問題のあるデバイス** タイルはセキュリティ運用ダッシュボードにあります。 このタイルは、センサー データを提供し、Defender for Endpoint サービスと通信する個々のデバイスの能力に関する情報を提供します。 注意が必要なデバイスの数が報告され、問題のあるデバイスを特定し、既知の問題を修正するためのアクションを取るのに役立ちます。

タイル上の 2 つの状態インジケーターは、サービスに正しく報告していないデバイスの数に関する情報を提供します。

- **間違った構成** Defender for Endpoint サービスにセンサー データを部分的に報告している可能性があるデバイスに、修正が必要な構成エラーがある可能性があります。
- **非アクティブ** 過去 1 か月間で 7 日以上、Defender for Endpoint サービスへの報告が停止したデバイス。

いずれかのグループをクリックすると、選択した内容に応じてフィルター処理されたデバイスの一覧が表示されます。 デバイス リストでは、以下の状態で正常性状態の一覧をいるター処理できます。

- **アクティブ** Defender for Endpoint サービスにアクティブに報告しているデバイス。
- **間違った構成** デバイスが Defender for Endpoint サービスにセンサー データを部分的に報告している場合でも、修正が必要な構成エラーがある可能性があります。 間違って構成されたデバイスには、次のような問題のいずれかまたは組み合わせがあります。

    - センサー データなし - デバイスがセンサー データの送信を停止しました。 制限のあるアラートをデバイスでトリガーすることができます。
    - 障害のある通信 - デバイスとの通信機能に障害が発生しています。 詳細分析のためのファイルの送信、ファイルのブロック、ネットワークからのデバイスの分離など、デバイスとの通信を必要とするアクションが機能しない場合があります。
- **アクティブ** Defender for Endpoint サービスへの報告を停止しているデバイス。

エクスポート機能を使用して、すべてのリストを CSV 形式でダウンロードすることができます。

詳細については、「[Microsoft Defender for Endpoint のセンサーの正常性状態をチェックする](/microsoft-365/security/defender-endpoint/check-sensor-status)」を参照してください。

デバイスが非アクティブまたは間違った設定になった原因の詳細については、「[Microsoft Defender for Endpoint で問題が発生したセンサーの修正](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)」を参照してください。

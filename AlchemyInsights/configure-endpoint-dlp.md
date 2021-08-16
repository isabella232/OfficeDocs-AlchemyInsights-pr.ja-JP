---
title: エンドポイント DLP を構成する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: f29d8476881fb3f93b369c057efed0acdd2169baf956ab43bf3c0ade527e9437
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033535"
---
# <a name="configure-endpoint-dlp"></a>エンドポイント DLP を構成する

Microsoft エンドポイント DLP を使用すると、 DLP の保護およびモニタリング機能を Windows 10 デバイス上の機密情報にまで拡張できます。 デバイスがデバイス管理に組み込まれたら、DLP ポリシーを作成してアイテムに保護アクションを適用できます。 アクティビティ エクスプローラーを使用して、機密アイテムのアクティビティを監視できます。 詳細については、「[デバイス管理にデバイスを組み込む](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)」を参照してください。  

エンドポイント DLP の使用を開始するには:

- 適切な SKU/サブスクリプションライセンスがあることを確認します。 詳細については、「[SKU/サブスクリプションライセンス](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)」を参照してください。
- デバイス管理を有効にしたり、オンボーディング ページにアクセスしたり、デバイス監視をオン/オフするために必要なアクセス許可を確認します。詳細は「[アクセス許可](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)」を参照してください。
- オンボーディング デバイスの手順に従って、デバイスをデバイス管理に組み込みことができます。 詳細については、「[オンボーディング デバイス](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)」を参照してください。 
- 機密アイテムを保護する DLP ポリシーを作成します。 詳細については、「[エンドポイント DLP ポリシーのシナリオ](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)」を参照してください。

Microsoft エンドポイント DLP の詳細については、「[Microsoft 365 エンドポイントのデータ損失防止について学ぶ (プレビュー)](/microsoft-365/compliance/endpoint-dlp-learn-about) 」を参照してください。

**サポートが必要な場合の重要なデータ収集手順:**

1. [MDATP クライアント アナライザ プレビュー](https://aka.ms/betamdatpanalyzer)をダウンロードします。
1. cmd ウィンドウから管理者としてツールを次のように実行します。

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. **「トレースを収集する分数を入力してください:**」というプロンプトが表示されたら、シナリオの実行に必要な分数を入力します。
1. シナリオを実行します。

サポート エージェントに提供する Zip ファイル出力を収集します。

---
title: Edge ブラウザーを使用するとインジケーターが機能しない
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
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676609"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Edge ブラウザーを使用するとインジケーターが機能しない

インジケーターを作成した後、Edge (スマートスクリーン) によって受け入れられません。 詳細については、「[IP および URL/ドメインのインジケーターを作成する](/microsoft-365/security/defender-endpoint/indicator-ip-domain)」を参照してください。

## <a name="step-1-ensure-the-following"></a>手順 1: 次のことを確認する

- インジケーターが正しいことを確認します (IP/URL にタイプミスがないこと、正しいアクション、正しい RBAC グループ)。
- 潜在的な待機時間を考慮し、インジケーターを作成してから最低 2 時間待ちます。
- システムが Microsoft Defender for Endpoint にオンボードされていることを確認します。
- システムがクラウドと通信できることを確認します。
- [テスト サイト](https://demo.smartscreen.msft.net)に移動し、スマートスクリーンが有効になっていて到達可能であることを確認します。

## <a name="step-2-troubleshoot-the-potential-issue"></a>手順 2: 潜在的な問題のトラブルシューティング

- クライアントが要件を満たしていることを確認してください。 詳細については、「[IP および URL/ドメインのインジケーターを作成する](/microsoft-365/security/defender-endpoint/indicator-ip-domain)」を参照してください。
- Edge ブラウザーの最新バージョンを実行していることを確認してください。 最新バージョンを確認するには、「[お使いの Microsoft Edge のバージョンを確認する](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)」を参照してください。
- Edge ブラウザーを再起動します。
- インジケーターをセットアップしたサイトに移動します。 サイトが期待どおりに表示されない場合は、手順 3 に進みます。 

## <a name="step-3-collect-data"></a>手順 3: データを収集する

- **MDEClientAnalyzer** 診断データを収集します。 手順については、「[Microsoft Defender for Endpoints へのマシンのオンボードに関する問題](issues-with-onboarding-machines.md)」を参照してください。
- Fiddler トレースのインストールと収集に慣れている場合は、「[Telerik Fiddler](http://www.telerik.com/fiddler)」を参照してください。
- Microsoft サポートからのガイダンスを希望する場合は、下の [サポート] アイコンを選択してサポート ケースを開きます。

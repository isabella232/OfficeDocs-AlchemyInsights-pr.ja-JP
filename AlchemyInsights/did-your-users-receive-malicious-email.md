---
title: ユーザーが悪意のあるメールを受信した場合
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326680"
---
# <a name="did-your-users-receive-malicious-email"></a>ユーザーが悪意のあるメールを受信した場合

現在は、[[Microsoft 365 Defender ポータルの報告]](https://sip.security.microsoft.com/reportsubmission?viewid=admin) から、悪意のあるメールを Microsoft に報告することができます。

[管理者の報告](https://security.microsoft.com/reportsubmission?viewid=admin)に送信されたメッセージがスキャンされ、次の結果が詳細ポップアップに表示されます。

- 配信時に送信者のメール認証に失敗した場合。
- メッセージのセキュリティ判定に影響を与える、または上書きされる可能性があるポリシー ヒットに関する情報。
- 現在の爆発的な結果により、メッセージに含まれる URL またはファイルが悪意のあるものかが確認されます。
- 評価者からのフィードバック

上書きが見つかった場合、再スキャンは数分で完了します。メール認証に問題がなかった場合、または配信が上書きによる影響を受けなかった場合でも、評価者からのフィードバックは最大で 1 日かかる可能性があります。

メッセージ、URL またはファイル (ブロックされている場合とブロックされていない場合) の最終的な判断に同意できない場合は、再スキャンを行うために、1 日後にメッセージを再送信してください。 メッセージを再送信した後にセキュリティ判定が変わる可能性は十分ありえます。

その間、[この記事](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)の手順に従って、ユーザーの受信トレイから悪意のあるメールを削除します。

- Microsoft Defender for Office 365 をお使いのお客様は次のサービスを利用できます。
  - [脅威エクスプローラーを使って不審なメールを検索して削除する](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [安全なリンクを使用して悪意のある URL アクセスをブロックする](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links)
  - 悪意のある URL をクリックしてアクセスしたユーザーを追跡する: [フィッシング URL を表示して、セキュリティ判定データをクリックします。](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - 手動にて[自動調査を開始する](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

「[悪意のある URL およびファイルからの保護](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)」の手順に従って、悪意のあるファイルおよび URL からの保護を行うこともできます。

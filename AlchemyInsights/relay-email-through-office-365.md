---
title: Microsoft 365 経由の中継メール
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: f02daad7d4b4a11f8d8bb1ef1467db5809cbd291
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324367"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>多機能デバイスまたはアプリケーションを設定して、メールを送信します

オプションおよび手順の詳細については、「[多機能デバイスまたはアプリケーションを設定して、Microsoft 365 を使用してメールを送信する方法](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)」を参照してください。
  
最近動作を停止したデバイスまたはアプリケーションがある場合、最も一般的な問題は次のとおりです。

- **SMTP 認証クライアント送信を使用時の認証関連エラー** 最近、SMTP 認証の動作に関連するいくつかの変更を行いました。 問題を解決する方法の詳細については、「[Microsoft 365 または Office 365 を使用して電子メールを送信するプリンター、スキャナー、および LOB アプリケーションの問題を修正する](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)」の「認証失敗」セクションを参照してください。
- **Office 365 へのセキュリティで保護された接続を行っている間は TLS 1.2 バージョンのみを受け入れます** セキュリティで保護された接続 (TLS) を使用している場合は、アプリケーション デバイスで TLS 1.2 がサポートされていることを確認してください。 詳細については、「[Microsoft 365 および Office 365 GCC での TLS 1.2 の準備](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)」を参照してください。
 
その他の問題と解決策については、「[Microsoft 365 または Office 365 を使用して電子メールを送信するプリンター、スキャナー、および LOB アプリケーションの問題を解決する](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)」を参照してください。

影響を受けるデバイスを確認するには、「[SMTP Auth クライアントのレポート](https://protection.office.com/mailflow/dashboard)」に移動します。

**注**: Exchange Online では、一括メールのシナリオには対応できません。一括商用メール (顧客ニュースレターなど) を送信するには、これらのサービスを専門とするサード パーティのプロバイダーを使用する必要があります。

---
title: Microsoft 365 メール サービスの SMTP 設定
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 2caa5d8ed9525129b66cc362b8b40149629006ba
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325980"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>Microsoft 365 メール サービスの SMTP 設定

Microsoft 365 メール サービスの SMTP 設定は次のとおりです。

**サーバー**: smtp.office365.com </br>
**ポート**: 587 </br>
**暗号化**: STARTTLS (現在は TLS 1.2 バージョンのみがサポートされています。 アプリケーションまたはデバイスが TLS 1.2 をサポートしていることを確認してください) </br>
**ユーザー名**: Office 365 アドレス (例: example@yourdomain.com) </br>
**パスワード**: Office 365 のパスワード </br>
**認証**: 必須 </br>
**送信制限**: 1 日 10,000 通のメール </br>

POP および IMAP の設定については、「[POP、IMAP、および SMTP の設定](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353)」を参照してください。
 
Microsoft 365 を使用してメールを中継するオプションと手順については、「[Microsoft 365 または Office 365 を使用してメールを送信するように多機能デバイスまたはアプリケーションをセットアップする方法](https://docs.microsoft.com/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)」を参照してください。
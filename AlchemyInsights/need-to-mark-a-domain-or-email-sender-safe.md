---
title: ドメインまたはメール送信者に安全マークを付ける必要がありますか?
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
- "9002921"
- "5673"
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319953"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>ドメインまたはメール送信者に安全マークを付ける必要がありますか?

- 組織がスパム、フィッシング、なりすまし攻撃にさらされる可能性があるため、**差出人セーフ リストの使用は推奨されません**。
- ただし、ビジネス要件がある場合は、**[メール フロー ルール](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** を使用することを **お勧めします**。 私たちのガイダンスは、送信者の認証を保証します (送信ドメインがなりすましではないことを確認します)。 
    **注**: スパム フィルター処理の例外により、組織がセキュリティ攻撃を受ける可能性があるため、差出人セーフ リストを使用して誤検知を管理することはお勧めしません。 ユーザーが誤って迷惑メールまたは迷惑メールとしてマーク付けされたメッセージを受信した場合は、**[メッセージとファイルを Microsoft に報告してください](https://protection.office.com/reportsubmission)**。
- Outlook の差出人セーフ リスト、スパム対策ポリシーで許可された送信者リスト、または許可されたドメイン リストは、送信者がすべてのスパム、なりすまし、フィッシング保護、送信者認証 (SPF、DKIM、DMARC) をバイパスするため、**避ける必要があります**。このメソッドは一時的な試験にのみ使用するためのものです。
- 特定のメールでスパム対策の評価がバイパスされる検証については、"X-Forefront-Antispam-Report" メッセージ ヘッダー (SFV:SFE、SFV:SKA、SFV:SAF) を確認して、**[スパム対策メッセージ ヘッダー](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** を参照してください。
- Microsoft は、お客様の[セキュリティを既定](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)に維持する必要があるため、マルウェアや確率性の高いフィッシングには一部のテナントによる上書きは適用されません。 これらの上書きは次のとおりです。o   許可された送信者リストまたは許可されたドメイン一覧 (スパム対策ポリシー) o   Outlook の差出人セーフ リスト o   IP 許可リスト (接続フィルター処理) 
- フィッシングの確率が高いメッセージのフィルター処理をバイパスできる唯一の上書きは、Exchange メールフロー ルール (トランスポート ルールとも呼ばれる) です。 メール フロー ルールを使用してフィルター処理をバイパスする方法については、「**[メール フロー ルールを使用して、フィルター処理のメッセージにスパムの信頼度 (SCL) を設定する](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**」をご覧ください。
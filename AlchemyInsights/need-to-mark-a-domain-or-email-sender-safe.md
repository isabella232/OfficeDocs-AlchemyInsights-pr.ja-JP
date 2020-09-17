---
title: ドメインまたはメール送信者に安全マークを付ける必要がありますか?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803250"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>ドメインまたはメール送信者に安全マークを付ける必要がありますか?

- 組織がスパム、フィッシング、なりすまし攻撃にさらされる可能性があるため、**差出人セーフ リストの使用は推奨されません**。
- ただし、ビジネス要件がある場合は、**[メール フロー ルール](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** を使用することを**お勧めします**。 私たちのガイダンスは、送信者の認証を保証します (送信ドメインがなりすましではないことを確認します)。 **注**: スパム フィルター処理の例外により、組織がセキュリティ攻撃を受ける可能性があるため、差出人セーフ リストを使用して誤検知を管理することはお勧めしません。 ユーザーが誤って迷惑メールまたは迷惑メールとしてマーク付けされたメッセージを受信した場合は、**[メッセージとファイルを Microsoft に報告してください](https://protection.office.com/reportsubmission)**。
- Outlook の差出人セーフ リスト、スパム対策ポリシーの許可された送信者リスト、または許可されたドメイン リストは、送信者がすべてのスパム、なりすまし、フィッシング保護、送信者認証 (SPF、DKIM、DMARC) をバイパスするため、**避ける必要があります**。 この方法は、一時的なテストのみに最適です。

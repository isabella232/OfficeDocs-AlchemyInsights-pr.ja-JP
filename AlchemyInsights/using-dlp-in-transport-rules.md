---
title: トランスポート ルールで DLP を使用する
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
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827221"
---
# <a name="using-dlp-in-transport-rules"></a>トランスポート ルールで DLP を使用する

データ損失防止 (DLP) を既存のトランスポートに統合するには、トランスポート ルールの設定で "**If the message contains...Sensitive Information**" (メッセージに...機密情報が含まれる場合) の条件を使用します。

**詳細については、次を参照してください。**

- トランスポート ルールでの統合された DLP 機密情報の種類: [機密情報ルールを統合する](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)。

このルールでテスト モードを使用して、ポリシー テストあり、またはポリシー テストなしで、ルールをテストすることもできます。  ルールを作成してからテストするまで、30 分待つ必要があります。

- 「[メール フロー/トランスポート ルールをテストする](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)」を参照してください。

**注**: トランスポート ルールを使用して新しい DLP ポリシーを EAC に実装する場合は、代わりに、[セキュリティ/コンプライアンスセンターで DLP ポリシー](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide)を使用します。

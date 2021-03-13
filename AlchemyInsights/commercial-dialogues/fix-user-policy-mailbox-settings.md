---
title: ユーザー ポリシー/メールボックスの設定を修正する
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751414"
---
# <a name="fix-user-policymailbox-settings"></a>ユーザー ポリシー/メールボックスの設定を修正する

メールボックスの迷惑メールの設定は、このメッセージに影響しました。 設定を確認するには、次の操作を行います。

1. Exchange 管理シェルを起動します。 詳細については、「[Exchange 管理シェルを開く](https://go.microsoft.com/fwlink/?linkid=2101432)」を参照してください。
2. 次のコマンドを実行します (ユーザーのメール アドレスを使用):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. 送信者のメール アドレスが **TrustedSendersAndDomains** または **BlockedSendersAndDomains** の一部であるかを確認してください。 メール アドレスがリストにある場合は、削除する必要がある場合があります。 詳細については、[Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047) を参照してください。

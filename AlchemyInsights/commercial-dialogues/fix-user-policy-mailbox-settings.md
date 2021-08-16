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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034723"
---
# <a name="fix-user-policymailbox-settings"></a>ユーザー ポリシー/メールボックスの設定を修正する

メールボックスの迷惑メールの設定は、このメッセージに影響しました。 設定を確認するには、次の操作を行います。

1. Exchange 管理シェルを起動します。 詳細については、「[Exchange 管理シェルを開く](https://go.microsoft.com/fwlink/?linkid=2101432)」を参照してください。
2. 次のコマンドを実行します (ユーザーのメール アドレスを使用):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. 送信者のメール アドレスが **TrustedSendersAndDomains** または **BlockedSendersAndDomains** の一部であるかを確認してください。 メール アドレスがリストにある場合は、削除する必要がある場合があります。 詳細については、[Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047) を参照してください。

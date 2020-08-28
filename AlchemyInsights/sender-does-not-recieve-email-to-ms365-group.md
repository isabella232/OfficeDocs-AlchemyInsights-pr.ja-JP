---
title: 送信者が Microsoft 365 グループに送信されたメールを受信しない
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872358"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>送信者が Microsoft 365 グループに送信されたメールを受信しない

既定では、Microsoft 365 グループへのメール メッセージの送信者は、送信者がグループのメンバーであっても、受信トレイでメッセージのコピーを受信しません。

次の EXO PowerShell コマンドを使用して、送信者が Microsoft 365 グループに送信する各メールのコピーを受信できるようにします。  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

すべてのメールボックスの設定を一度に有効にするには:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**注** この設定への変更は、反映されるまで最大 1 時間かかります。
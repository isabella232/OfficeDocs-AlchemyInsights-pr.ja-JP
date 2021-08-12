---
title: 送信者が Microsoft 365 グループに送信されたメールを受信しない
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 893b80567567590357a638370b8c8d58b87a98a51c68cfcc84629eda5ac71b44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958302"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>送信者が Microsoft 365 グループに送信されたメールを受信しない

既定では、Microsoft 365 グループへのメール メッセージの送信者は、送信者がグループのメンバーであっても、受信トレイでメッセージのコピーを受信しません。

次の EXO PowerShell コマンドを使用して、送信者が Microsoft 365 グループに送信する各メールのコピーを受信できるようにします。  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

すべてのメールボックスの設定を一度に有効にするには:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**注** この設定への変更は、反映されるまで最大 1 時間かかります。
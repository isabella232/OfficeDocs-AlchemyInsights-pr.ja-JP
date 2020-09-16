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
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751320"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="7bf14-102">送信者が Microsoft 365 グループに送信されたメールを受信しない</span><span class="sxs-lookup"><span data-stu-id="7bf14-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="7bf14-103">既定では、Microsoft 365 グループへのメール メッセージの送信者は、送信者がグループのメンバーであっても、受信トレイでメッセージのコピーを受信しません。</span><span class="sxs-lookup"><span data-stu-id="7bf14-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="7bf14-104">次の EXO PowerShell コマンドを使用して、送信者が Microsoft 365 グループに送信する各メールのコピーを受信できるようにします。</span><span class="sxs-lookup"><span data-stu-id="7bf14-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="7bf14-105">すべてのメールボックスの設定を一度に有効にするには:</span><span class="sxs-lookup"><span data-stu-id="7bf14-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="7bf14-106">**注** この設定への変更は、反映されるまで最大 1 時間かかります。</span><span class="sxs-lookup"><span data-stu-id="7bf14-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>
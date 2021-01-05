---
title: Microsoft 365 グループに送信されたメールに対して受信した AggregateGroupMailbox の完全な NDR
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722213"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a><span data-ttu-id="cd90f-102">Microsoft 365 グループに送信されたメールに対して受信した AggregateGroupMailbox の完全な NDR</span><span class="sxs-lookup"><span data-stu-id="cd90f-102">AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group</span></span>

<span data-ttu-id="cd90f-103">次の EXO シェル コマンドを使用して、Exchange トランスポート ルールを作成し、集約グループのメールボックスに送信されたメールをサイレントにドロップします。</span><span class="sxs-lookup"><span data-stu-id="cd90f-103">Use the following EXO Shell command to create an Exchange transport rule to silently drop emails sent to aggregate group mailbox:</span></span>

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> <span data-ttu-id="cd90f-104">**-SentTo** の SMTP アドレスを、テナントの集約グループのメールボックスの SMTP アドレスに置き換えます。</span><span class="sxs-lookup"><span data-stu-id="cd90f-104">Replace the SMTP address in **-SentTo** with SMTP address of aggregate group mailbox in your tenant.</span></span> <span data-ttu-id="cd90f-105">受信した NDR から集約グループのメールボックスの SMTP アドレスを取得できます。</span><span class="sxs-lookup"><span data-stu-id="cd90f-105">You can get the SMTP address of aggregate group mailbox from the NDR received.</span></span>




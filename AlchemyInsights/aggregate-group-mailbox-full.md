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
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Microsoft 365 グループに送信されたメールに対して受信した AggregateGroupMailbox の完全な NDR

次の EXO シェル コマンドを使用して、Exchange トランスポート ルールを作成し、集約グループのメールボックスに送信されたメールをサイレントにドロップします。

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> **-SentTo** の SMTP アドレスを、テナントの集約グループのメールボックスの SMTP アドレスに置き換えます。 受信した NDR から集約グループのメールボックスの SMTP アドレスを取得できます。




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
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315915"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Microsoft 365 グループに送信されたメールに対して受信した AggregateGroupMailbox の完全な NDR

次の EXO シェル コマンドを使用して、Exchange トランスポート ルールを作成し、集約グループのメールボックスに送信されたメールをサイレントにドロップします。

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**注**: **-SentTo** の SMTP アドレスを、テナントの集約グループのメールボックスの SMTP アドレスに置き換えます。 受信した NDR から集約グループのメールボックスの SMTP アドレスを取得できます。




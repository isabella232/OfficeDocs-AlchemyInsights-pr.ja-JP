---
title: 'Microsoft 365 グループに送信されるすべての電子メールの自動返信を構成するには:'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: 1adc3c131daedb26d88710f4b4078b0622ad13c5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331536"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>Microsoft 365 グループに送信されるすべての電子メールの自動返信を構成するには:

**テナント管理者アカウントを使用して EXO PowerShell に接続し、次のコマンドを使用します**。

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

**注**: **groupmailbox** を、自動応答を構成するグループ名に変更します。


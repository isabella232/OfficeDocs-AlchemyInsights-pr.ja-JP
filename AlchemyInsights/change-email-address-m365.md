---
title: Microsoft 365 グループのメール アドレスを変更する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/10/2020
ms.locfileid: "48462097"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 グループのメール アドレスを変更する

管理センターを使用して、Microsoft 365 グループのメール アドレスを変更することができます。 グループを選択し、「メール アドレスを編集する」を選択します。

次の EXO PowerShell コマンドを使用して、Microsoft 365 グループのプライマリ SMTP アドレスを変更することもできます。

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

例:

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`

---
title: Microsoft 365 グループのメール アドレスを変更する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/27/2020
ms.locfileid: "43911315"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Microsoft 365 グループのメール アドレスを変更する

管理センターを使用して、Microsoft 365 グループのメール アドレスを変更することができます。 グループを選択し、「メール アドレスを編集する」を選択します。

次の EXO PowerShell コマンドを使用して、Microsoft 365 グループのプライマリ SMTP アドレスを変更することもできます。

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

例:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```

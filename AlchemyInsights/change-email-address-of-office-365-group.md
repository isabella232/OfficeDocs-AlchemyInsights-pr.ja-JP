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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580662"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 グループのメール アドレスを変更する

管理センターを使用して、Microsoft 365 グループのメール アドレスを変更することができます。 グループを選択し、「メール アドレスを編集する」を選択します。

次の EXO PowerShell コマンドを使用して、Microsoft 365 グループのプライマリ SMTP アドレスを変更することもできます。

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

例:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```

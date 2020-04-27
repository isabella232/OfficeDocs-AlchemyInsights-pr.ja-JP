---
title: Office 365 グループのメール アドレスを変更する
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
ms.openlocfilehash: 72f02bec6f8cd61f7c5ab202abb21f41aa9f549d
ms.sourcegitcommit: f7f25506191d0656a7637340df806b82c4232bc4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/21/2020
ms.locfileid: "43599218"
---
# <a name="change-email-address-of-an-office-365-group"></a>Office 365 グループのメール アドレスを変更する

管理センターを使用して、Office 365 グループのメール アドレスを変更することができます。 グループを選択し、「メール アドレスを編集する」を選択します。

次の EXO PowerShell コマンドを使用して、Office 365 グループのプライマリ SMTP アドレスを変更することもできます。

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

例:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```

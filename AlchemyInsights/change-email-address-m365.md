---
title: Microsoft 365 グループまたは Microsoft Teams のメール アドレスを変更する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819085"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Microsoft 365 グループまたは Microsoft Teams のメール アドレスを変更する

Microsoft 365 グループまたは Microsoft Teams のメール アドレスは、[Microsoft 365 管理センター](https://admin.microsoft.com/)を使用して変更できます。 グループを選択し、「メール アドレスを編集する」を選択します。

次の EXO PowerShell コマンドを使用して、Microsoft 365 グループまたは Teams のプライマリ SMTP アドレスを変更することもできます。

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

例:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`

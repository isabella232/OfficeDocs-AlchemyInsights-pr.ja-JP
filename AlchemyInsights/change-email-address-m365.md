---
title: Microsoft 365 グループまたは Microsoft Teams のメール アドレスを変更する
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756562"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Microsoft 365 グループまたは Microsoft Teams のメール アドレスを変更する

Microsoft 365 グループまたは Microsoft Teams のメール アドレスは、[Microsoft 365 管理センター](https://admin.microsoft.com/)を使用して変更できます。 グループを選択し、「メール アドレスを編集する」を選択します。

次の EXO PowerShell コマンドを使用して、Microsoft 365 グループまたは Teams のプライマリ SMTP アドレスを変更することもできます。

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

例:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`

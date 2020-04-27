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
# <a name="change-email-address-of-an-office-365-group"></a><span data-ttu-id="1c37e-102">Office 365 グループのメール アドレスを変更する</span><span class="sxs-lookup"><span data-stu-id="1c37e-102">Change email address of an Office 365 group</span></span>

<span data-ttu-id="1c37e-103">管理センターを使用して、Office 365 グループのメール アドレスを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="1c37e-103">You can change the email address of an Office 365 group by using the admin center.</span></span> <span data-ttu-id="1c37e-104">グループを選択し、「メール アドレスを編集する」を選択します。</span><span class="sxs-lookup"><span data-stu-id="1c37e-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="1c37e-105">次の EXO PowerShell コマンドを使用して、Office 365 グループのプライマリ SMTP アドレスを変更することもできます。</span><span class="sxs-lookup"><span data-stu-id="1c37e-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Office 365 group:</span></span>

<span data-ttu-id="1c37e-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="1c37e-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="1c37e-107">例:</span><span class="sxs-lookup"><span data-stu-id="1c37e-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```

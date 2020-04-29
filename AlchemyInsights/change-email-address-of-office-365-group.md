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
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="eb16e-102">Microsoft 365 グループのメール アドレスを変更する</span><span class="sxs-lookup"><span data-stu-id="eb16e-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="eb16e-103">管理センターを使用して、Microsoft 365 グループのメール アドレスを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="eb16e-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="eb16e-104">グループを選択し、「メール アドレスを編集する」を選択します。</span><span class="sxs-lookup"><span data-stu-id="eb16e-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="eb16e-105">次の EXO PowerShell コマンドを使用して、Microsoft 365 グループのプライマリ SMTP アドレスを変更することもできます。</span><span class="sxs-lookup"><span data-stu-id="eb16e-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="eb16e-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="eb16e-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="eb16e-107">例:</span><span class="sxs-lookup"><span data-stu-id="eb16e-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```

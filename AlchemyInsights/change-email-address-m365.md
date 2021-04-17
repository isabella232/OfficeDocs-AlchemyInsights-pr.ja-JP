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
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="9a13d-102">Microsoft 365 グループまたは Microsoft Teams のメール アドレスを変更する</span><span class="sxs-lookup"><span data-stu-id="9a13d-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="9a13d-103">Microsoft 365 グループまたは Microsoft Teams のメール アドレスは、[Microsoft 365 管理センター](https://admin.microsoft.com/)を使用して変更できます。</span><span class="sxs-lookup"><span data-stu-id="9a13d-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="9a13d-104">グループを選択し、「メール アドレスを編集する」を選択します。</span><span class="sxs-lookup"><span data-stu-id="9a13d-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="9a13d-105">次の EXO PowerShell コマンドを使用して、Microsoft 365 グループまたは Teams のプライマリ SMTP アドレスを変更することもできます。</span><span class="sxs-lookup"><span data-stu-id="9a13d-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="9a13d-106">例:</span><span class="sxs-lookup"><span data-stu-id="9a13d-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`

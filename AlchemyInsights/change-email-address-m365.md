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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="deada-102">Microsoft 365 グループのメール アドレスを変更する</span><span class="sxs-lookup"><span data-stu-id="deada-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="deada-103">管理センターを使用して、Microsoft 365 グループのメール アドレスを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="deada-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="deada-104">グループを選択し、「メール アドレスを編集する」を選択します。</span><span class="sxs-lookup"><span data-stu-id="deada-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="deada-105">次の EXO PowerShell コマンドを使用して、Microsoft 365 グループのプライマリ SMTP アドレスを変更することもできます。</span><span class="sxs-lookup"><span data-stu-id="deada-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="deada-106">例: </span><span class="sxs-lookup"><span data-stu-id="deada-106">Example:</span></span>

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`

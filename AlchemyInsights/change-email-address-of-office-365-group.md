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
ms.openlocfilehash: a2605bcd66f61de811ebb6e273e4ef1cff2b0119
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47733692"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="30fb5-102">Microsoft 365 グループのメール アドレスを変更する</span><span class="sxs-lookup"><span data-stu-id="30fb5-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="30fb5-103">管理センターを使用して、Microsoft 365 グループのメール アドレスを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="30fb5-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="30fb5-104">グループを選択し、「メール アドレスを編集する」を選択します。</span><span class="sxs-lookup"><span data-stu-id="30fb5-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="30fb5-105">次の EXO PowerShell コマンドを使用して、Microsoft 365 グループのプライマリ SMTP アドレスを変更することもできます。</span><span class="sxs-lookup"><span data-stu-id="30fb5-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="30fb5-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="30fb5-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="30fb5-107">例:</span><span class="sxs-lookup"><span data-stu-id="30fb5-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```

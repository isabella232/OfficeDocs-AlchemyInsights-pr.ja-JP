---
title: メールボックスの監査を有効にする
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: c04f27edc1e22e0e4269758827d5468767967be8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814197"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="926e6-102">メールボックスの監査を有効にする</span><span class="sxs-lookup"><span data-stu-id="926e6-102">Enable mailbox auditing</span></span>

<span data-ttu-id="926e6-103">メールボックスの監査を 1 人のユーザーまたは組織全体に対して有効にするには、リモート PowerShell から以下のコマンドレットを実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="926e6-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="926e6-104">**1 人のユーザー**</span><span class="sxs-lookup"><span data-stu-id="926e6-104">**Single User**</span></span>
  
<span data-ttu-id="926e6-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="926e6-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="926e6-106">**組織**</span><span class="sxs-lookup"><span data-stu-id="926e6-106">**Organization**</span></span>
  
<span data-ttu-id="926e6-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="926e6-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="926e6-108">詳細情報</span><span class="sxs-lookup"><span data-stu-id="926e6-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  


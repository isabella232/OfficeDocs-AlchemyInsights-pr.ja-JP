---
title: メールボックスの監査を有効にする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297103"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="da918-102">メールボックスの監査を有効にする</span><span class="sxs-lookup"><span data-stu-id="da918-102">Enable mailbox auditing</span></span>

<span data-ttu-id="da918-103">1 人のユーザーまたは組織全体のいずれかのメールボックスの監査を有効にするには、電源のリモート シェルから次のコマンドレットを実行してください。</span><span class="sxs-lookup"><span data-stu-id="da918-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="da918-104">**1 人のユーザー**</span><span class="sxs-lookup"><span data-stu-id="da918-104">**Single User**</span></span>
  
<span data-ttu-id="da918-105">セット-メールボックスの識別情報"Jane Dow"AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="da918-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="da918-106">**組織**</span><span class="sxs-lookup"><span data-stu-id="da918-106">**Organization**</span></span>
  
<span data-ttu-id="da918-107">Get メールボックス ResultSize 無制限-{RecipientTypeDetails - eq「構成」} のフィルターを適用します。$True を設定メールボックス AuditEnabled</span><span class="sxs-lookup"><span data-stu-id="da918-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="da918-108">詳細情報</span><span class="sxs-lookup"><span data-stu-id="da918-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  


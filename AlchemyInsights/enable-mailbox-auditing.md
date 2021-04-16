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
# <a name="enable-mailbox-auditing"></a>メールボックスの監査を有効にする

メールボックスの監査を 1 人のユーザーまたは組織全体に対して有効にするには、リモート PowerShell から以下のコマンドレットを実行する必要があります。
  
 **1 人のユーザー**
  
Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
  
 **組織**
  
Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true
  
[詳細情報](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  


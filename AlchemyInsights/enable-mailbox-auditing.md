---
title: メールボックスの監査を有効にする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736258"
---
# <a name="enable-mailbox-auditing"></a>メールボックスの監査を有効にする

メールボックスの監査を 1 人のユーザーまたは組織全体に対して有効にするには、リモート PowerShell から以下のコマンドレットを実行する必要があります。
  
 **1 人のユーザー**
  
Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
  
 **組織**
  
Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true
  
[詳細情報](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  


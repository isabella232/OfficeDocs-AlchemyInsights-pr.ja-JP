---
title: Microsoft 365 グループの「ようこそ」 メッセージ
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
- "5685"
ms.openlocfilehash: de16ca6021441bf6cb781106b7f3da8eed86b0f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725844"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Microsoft 365 グループの「ようこそ」 メッセージ

"UnifiedGroupWelcomeMessageEnabled" プロパティが True の場合は、Microsoft 365 グループに参加する新しいユーザーに、「ようこそ」メールが送信されます。

ウェルカム メッセージを無効にする場合は、次の [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) コマンドを使用します。

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`

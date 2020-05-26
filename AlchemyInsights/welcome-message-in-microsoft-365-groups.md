---
title: Microsoft 365 グループの「ようこそ」 メッセージ
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
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358725"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Microsoft 365 グループの「ようこそ」 メッセージ

"UnifiedGroupWelcomeMessageEnabled" プロパティが True の場合は、Microsoft 365 グループに参加する新しいユーザーに、「ようこそ」メールが送信されます。

ウェルカム メッセージを無効にする場合は、次の [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) コマンドを使用します。

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`

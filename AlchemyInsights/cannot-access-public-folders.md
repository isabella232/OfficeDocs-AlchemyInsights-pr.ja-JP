---
title: パブリック フォルダーにアクセスできません
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/10/2019
ms.locfileid: "39976360"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook はパブリック フォルダーに接続できません

パブリック フォルダー アクセスが少数のユーザーに対して機能しない場合には、以下を試してください。

EXO PowerShell に接続し、問題のあるユーザー アカウントの DefaultPublicFolderMailbox を、動作中のユーザー アカウントの DefaultPublicFolderMailbox と一致するように構成します。

例:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

変更が有効になるまで、少なくとも 1 時間待ちます。
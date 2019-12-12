---
title: パブリックフォルダーにアクセスできない
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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/10/2019
ms.locfileid: "39976360"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook がパブリックフォルダーに接続できない

パブリックフォルダーアクセスが少数のユーザーに対して機能しない場合は、次のことを試してください。

EXO PowerShell に接続し、問題のユーザーアカウントの DefaultPublicFolderMailbox を、作業中のユーザーアカウントの1つに一致するように構成します。

例:

WorkingUser の取得 |ft DefaultPublicFolderMailbox、EffectivePublicFolderMailbox

Set-Mailbox のプロパティ-以前のコマンド> \<からのユーザー-DefaultPublicFolderMailbox の値

変更を有効にするには、少なくとも1時間待つ必要があります。
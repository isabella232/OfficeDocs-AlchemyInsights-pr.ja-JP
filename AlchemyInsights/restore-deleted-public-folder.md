---
title: 削除されたパブリック フォルダーを復元する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943380"
---
# <a name="restore-a-deleted-public-folder"></a>削除されたパブリック フォルダーを復元する

**パブリック フォルダーから削除されたアイテムを復元するには**:

- 「[You can't recover deleted items from a non-mail public folder in Outlook 2016 (Outlook 2016 でメール以外のパブリック フォルダーから削除済みアイテムを復元することはできません)](https://aka.ms/pfrec)」を参照してください。
 
**(任意の種類の) 削除されたパブリック フォルダーを復元するには**: 

- 次の EXO PowerShell コマンドを使用してください。

    構文:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    例: 次のコマンドは、Subfolder1 を復元して \Parent1 の下に配置します:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

詳細については、「[削除されたパブリック フォルダーを復元する](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)」を参照してください。

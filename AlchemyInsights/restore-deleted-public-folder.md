---
title: 削除されたパブリックフォルダーを復元する
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
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2020
ms.locfileid: "42094390"
---
# <a name="restore-a-deleted-public-folder"></a>削除されたパブリックフォルダーを復元する

**パブリックフォルダーから削除済みアイテムを復元するには、次のようにし**ます。

- [Outlook 2016 のメール以外のパブリックフォルダーから削除済みアイテムを復元できないことを](https://aka.ms/pfrec)確認してください。
 
**削除されたパブリックフォルダー (任意の種類) を復元するには、次のようにし**ます。 

- 次の EXO PowerShell コマンドを使用してください。

    構文:

    >$pf = New-publicfolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-再帰 |?{$_.Name-eq "\<name_of_deleted_public_Folder"};$Pf New-publicfolder-フォルダーが復元される\<場所のパスパス>

    例: 次のコマンドは、Subfolder1 を復元し、親の下に配置します。

    >$pf = New-publicfolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-再帰 |?{$_.Name-eq "Subfolder1"};New-publicfolder $pf。 identity-Path/parent1

詳細について[は、「削除済みのパブリックフォルダーを復元する](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)」を参照してください。

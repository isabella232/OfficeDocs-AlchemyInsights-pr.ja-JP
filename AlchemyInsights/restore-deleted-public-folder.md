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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="dcab9-102">削除されたパブリックフォルダーを復元する</span><span class="sxs-lookup"><span data-stu-id="dcab9-102">Restore a deleted public folder</span></span>

<span data-ttu-id="dcab9-103">**パブリックフォルダーから削除済みアイテムを復元するには、次のようにし**ます。</span><span class="sxs-lookup"><span data-stu-id="dcab9-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="dcab9-104">[Outlook 2016 のメール以外のパブリックフォルダーから削除済みアイテムを復元できないことを](https://aka.ms/pfrec)確認してください。</span><span class="sxs-lookup"><span data-stu-id="dcab9-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="dcab9-105">**削除されたパブリックフォルダー (任意の種類) を復元するには、次のようにし**ます。</span><span class="sxs-lookup"><span data-stu-id="dcab9-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="dcab9-106">次の EXO PowerShell コマンドを使用してください。</span><span class="sxs-lookup"><span data-stu-id="dcab9-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="dcab9-107">構文:</span><span class="sxs-lookup"><span data-stu-id="dcab9-107">Syntax:</span></span>

    ><span data-ttu-id="dcab9-108">$pf = New-publicfolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-再帰 |?{$_.Name-eq "\<name_of_deleted_public_Folder"};$Pf New-publicfolder-フォルダーが復元される\<場所のパスパス></span><span class="sxs-lookup"><span data-stu-id="dcab9-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="dcab9-109">例: 次のコマンドは、Subfolder1 を復元し、親の下に配置します。</span><span class="sxs-lookup"><span data-stu-id="dcab9-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="dcab9-110">$pf = New-publicfolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-再帰 |?{$_.Name-eq "Subfolder1"};New-publicfolder $pf。 identity-Path/parent1</span><span class="sxs-lookup"><span data-stu-id="dcab9-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="dcab9-111">詳細について[は、「削除済みのパブリックフォルダーを復元する](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcab9-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>

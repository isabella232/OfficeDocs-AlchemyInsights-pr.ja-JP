---
title: 削除されたパブリック フォルダーを復元する
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
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158518"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="23da2-102">削除されたパブリック フォルダーを復元する</span><span class="sxs-lookup"><span data-stu-id="23da2-102">Restore a deleted public folder</span></span>

<span data-ttu-id="23da2-103">**パブリック フォルダーから削除されたアイテムを復元するには**:</span><span class="sxs-lookup"><span data-stu-id="23da2-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="23da2-104">「[You can't recover deleted items from a non-mail public folder in Outlook 2016 (Outlook 2016 でメール以外のパブリック フォルダーから削除済みアイテムを復元することはできません)](https://aka.ms/pfrec)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23da2-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="23da2-105">**(任意の種類の) 削除されたパブリック フォルダーを復元するには**:</span><span class="sxs-lookup"><span data-stu-id="23da2-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="23da2-106">次の EXO PowerShell コマンドを使用してください。</span><span class="sxs-lookup"><span data-stu-id="23da2-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="23da2-107">構文:</span><span class="sxs-lookup"><span data-stu-id="23da2-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="23da2-108">例: 次のコマンドは、Subfolder1 を復元して \Parent1 の下に配置します:</span><span class="sxs-lookup"><span data-stu-id="23da2-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="23da2-109">詳細については、「[削除されたパブリック フォルダーを復元する](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23da2-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>

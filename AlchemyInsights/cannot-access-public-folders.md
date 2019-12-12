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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="a9367-102">Outlook がパブリックフォルダーに接続できない</span><span class="sxs-lookup"><span data-stu-id="a9367-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="a9367-103">パブリックフォルダーアクセスが少数のユーザーに対して機能しない場合は、次のことを試してください。</span><span class="sxs-lookup"><span data-stu-id="a9367-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="a9367-104">EXO PowerShell に接続し、問題のユーザーアカウントの DefaultPublicFolderMailbox を、作業中のユーザーアカウントの1つに一致するように構成します。</span><span class="sxs-lookup"><span data-stu-id="a9367-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="a9367-105">例:</span><span class="sxs-lookup"><span data-stu-id="a9367-105">Example:</span></span>

<span data-ttu-id="a9367-106">WorkingUser の取得 |ft DefaultPublicFolderMailbox、EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="a9367-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="a9367-107">Set-Mailbox のプロパティ-以前のコマンド> \<からのユーザー-DefaultPublicFolderMailbox の値</span><span class="sxs-lookup"><span data-stu-id="a9367-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="a9367-108">変更を有効にするには、少なくとも1時間待つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9367-108">Wait at least one hour for the change to take effect.</span></span>
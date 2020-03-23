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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891754"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="e3491-102">Outlook はパブリック フォルダーに接続できません</span><span class="sxs-lookup"><span data-stu-id="e3491-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="e3491-103">パブリック フォルダー アクセスが一部のユーザーに対して機能しない場合には、以下を試してください。</span><span class="sxs-lookup"><span data-stu-id="e3491-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="e3491-104">EXO PowerShell に接続し、問題のあるユーザー アカウントの DefaultPublicFolderMailbox パラメーターを、動作中のユーザー アカウントのパラメーターと一致するように構成します。</span><span class="sxs-lookup"><span data-stu-id="e3491-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="e3491-105">例:</span><span class="sxs-lookup"><span data-stu-id="e3491-105">Example:</span></span>

<span data-ttu-id="e3491-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="e3491-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="e3491-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="e3491-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="e3491-108">変更が有効になるまで、少なくとも 1 時間待ちます。</span><span class="sxs-lookup"><span data-stu-id="e3491-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="e3491-109">問題が解決しない場合は、[この手順](https://aka.ms/pfcte)に従って、Outlook を使用したパブリック フォルダー アクセスの問題をトラブルシューティングしてください。</span><span class="sxs-lookup"><span data-stu-id="e3491-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
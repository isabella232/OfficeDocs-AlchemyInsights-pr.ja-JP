---
title: パブリック フォルダーにアクセスできません
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
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819517"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="d2555-102">Outlook はパブリック フォルダーに接続できません</span><span class="sxs-lookup"><span data-stu-id="d2555-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="d2555-103">パブリック フォルダー アクセスが一部のユーザーに対して機能しない場合には、以下を試してください。</span><span class="sxs-lookup"><span data-stu-id="d2555-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="d2555-104">EXO PowerShell に接続し、問題のあるユーザー アカウントの DefaultPublicFolderMailbox パラメーターを、動作中のユーザー アカウントのパラメーターと一致するように構成します。</span><span class="sxs-lookup"><span data-stu-id="d2555-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="d2555-105">例:</span><span class="sxs-lookup"><span data-stu-id="d2555-105">Example:</span></span>

<span data-ttu-id="d2555-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="d2555-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="d2555-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="d2555-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="d2555-108">変更が有効になるまで、少なくとも 1 時間待ちます。</span><span class="sxs-lookup"><span data-stu-id="d2555-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="d2555-109">問題が解決しない場合は、[この手順](https://aka.ms/pfcte)に従って、Outlook を使用したパブリック フォルダー アクセスの問題をトラブルシューティングしてください。</span><span class="sxs-lookup"><span data-stu-id="d2555-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="d2555-110">**Outlook を使用してパブリック フォルダーにアクセスできるユーザーを制御するには**:</span><span class="sxs-lookup"><span data-stu-id="d2555-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="d2555-111">SSet-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $falseを使用する</span><span class="sxs-lookup"><span data-stu-id="d2555-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="d2555-112">$true: ユーザーに Outlook のパブリック フォルダーへのアクセスを許可します</span><span class="sxs-lookup"><span data-stu-id="d2555-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="d2555-113">$false: ユーザーが Outlook のパブリック フォルダーにアクセスできないようにします。</span><span class="sxs-lookup"><span data-stu-id="d2555-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="d2555-114">これが既定値です。</span><span class="sxs-lookup"><span data-stu-id="d2555-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="d2555-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="d2555-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="d2555-116">**注**: この手順で制御できるのは、Windows クライアント用の Outlook デスクトップとの接続のみです。</span><span class="sxs-lookup"><span data-stu-id="d2555-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="d2555-117">ユーザーは OWA または Outlook for Mac を使用してパブリック フォルダーに引き続きアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="d2555-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="d2555-118">詳細については、[Outlookでのパブリックフォルダーへの制御された接続のサポートについてのお知らせ](https://aka.ms/controlpf)を をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d2555-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>
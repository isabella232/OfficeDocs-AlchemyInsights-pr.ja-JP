---
title: Outlook を使用してパブリック フォルダーへのアクセスを制御する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804405"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="e8730-102">Outlook を使用してパブリック フォルダーへのアクセスを制御する</span><span class="sxs-lookup"><span data-stu-id="e8730-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="e8730-103">Outlook を使用してパブリック フォルダーにアクセスできるユーザーを制御するには:</span><span class="sxs-lookup"><span data-stu-id="e8730-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="e8730-104">`Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` を使う</span><span class="sxs-lookup"><span data-stu-id="e8730-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="e8730-105">$true: ユーザーに Outlook のパブリック フォルダーへのアクセスを許可します</span><span class="sxs-lookup"><span data-stu-id="e8730-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="e8730-106">$false: ユーザーが Outlook のパブリック フォルダーにアクセスできないようにします。</span><span class="sxs-lookup"><span data-stu-id="e8730-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="e8730-107">これが既定値です。</span><span class="sxs-lookup"><span data-stu-id="e8730-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="e8730-108">注: この手順で制御できるのは、Windows クライアントの Outlook デスクトップとの接続のみです。</span><span class="sxs-lookup"><span data-stu-id="e8730-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="e8730-109">ユーザーは OWA または Outlook for Mac を使用してパブリック フォルダーに引き続きアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e8730-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="e8730-110">詳細については、「[Outlook のパブリック フォルダーへの制御された接続](https://aka.ms/controlpf)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8730-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>

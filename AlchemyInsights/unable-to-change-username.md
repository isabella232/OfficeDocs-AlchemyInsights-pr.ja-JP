---
title: ユーザー名を変更できません
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440595"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="17bb4-102">ユーザー名を変更できません</span><span class="sxs-lookup"><span data-stu-id="17bb4-102">Unable to change UserName</span></span>

<span data-ttu-id="17bb4-103">場合によっては、UPN (UserPrincipalName) の変更がクラウドに反映されないことがあります。</span><span class="sxs-lookup"><span data-stu-id="17bb4-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="17bb4-104">Office 365 ポータルで検証エラーが表示されるか、ユーザー名またはメールアドレスを変更できない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="17bb4-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="17bb4-105">この問題を解決するには、この PowerShell コマンドを使用して、手動で UserPrincipalName を設定します。</span><span class="sxs-lookup"><span data-stu-id="17bb4-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="17bb4-106">**例: ユーザー名を変更する**</span><span class="sxs-lookup"><span data-stu-id="17bb4-106">**Example: Rename a user**</span></span>

<span data-ttu-id="17bb4-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="17bb4-107">PowerShellCopy</span></span>

<span data-ttu-id="17bb4-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="17bb4-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="17bb4-109">このコマンドは、davidc@contoso.com を davidchew@contoso.com に変更します。</span><span class="sxs-lookup"><span data-stu-id="17bb4-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="17bb4-110">詳細については、[Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="17bb4-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>
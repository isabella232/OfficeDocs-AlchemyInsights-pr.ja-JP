---
title: 強力なパスワードの要件を変更する
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
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818473"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="f68bd-102">強力なパスワードの要件を変更する</span><span class="sxs-lookup"><span data-stu-id="f68bd-102">Change strong password requirement</span></span>

<span data-ttu-id="f68bd-103">既定では、 Microsoft は強力なパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="f68bd-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="f68bd-104">PowerShell で、次のコマンドを使用して、特定のユーザーに対して強力なパスワードを無効にすることができます:</span><span class="sxs-lookup"><span data-stu-id="f68bd-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="f68bd-105">すべてのユーザーに対して強力なパスワードを無効にするには、次を使用します:</span><span class="sxs-lookup"><span data-stu-id="f68bd-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="f68bd-106">パスワード ポリシーの詳細情報</span><span class="sxs-lookup"><span data-stu-id="f68bd-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="f68bd-107">PowerShell で Microsoft 365 に接続する方法</span><span class="sxs-lookup"><span data-stu-id="f68bd-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="f68bd-108">PowerShell MsolUser コマンドの詳細情報</span><span class="sxs-lookup"><span data-stu-id="f68bd-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)

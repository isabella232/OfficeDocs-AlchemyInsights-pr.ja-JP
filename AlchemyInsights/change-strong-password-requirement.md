---
title: 強力なパスワードの要件を変更する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518764"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="791e7-102">強力なパスワードの要件を変更する</span><span class="sxs-lookup"><span data-stu-id="791e7-102">Change strong password requirement</span></span>

<span data-ttu-id="791e7-103">Microsoft では、既定で強力なパスワードが必要になります。</span><span class="sxs-lookup"><span data-stu-id="791e7-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="791e7-104">PowerShell を使用すると、次のコマンドを使用して、特定のユーザーの強力なパスワードを無効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="791e7-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="791e7-105">*Get-msoluser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="791e7-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="791e7-106">パスワードポリシーの詳細情報</span><span class="sxs-lookup"><span data-stu-id="791e7-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="791e7-107">PowerShell を使用して Office 365 に接続する方法</span><span class="sxs-lookup"><span data-stu-id="791e7-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="791e7-108">PowerShell Get-msoluser コマンドの詳細情報</span><span class="sxs-lookup"><span data-stu-id="791e7-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
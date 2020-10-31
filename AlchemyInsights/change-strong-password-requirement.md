---
title: 強力なパスワードの要件を変更する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804428"
---
# <a name="change-strong-password-requirement"></a>強力なパスワードの要件を変更する

既定では、 Microsoft は強力なパスワードを要求します。

PowerShell で、次のコマンドを使用して、特定のユーザーに対して強力なパスワードを無効にすることができます:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

すべてのユーザーに対して強力なパスワードを無効にするには、次を使用します:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [パスワード ポリシーの詳細情報](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [PowerShell で Microsoft 365 に接続する方法](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [PowerShell MsolUser コマンドの詳細情報](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)

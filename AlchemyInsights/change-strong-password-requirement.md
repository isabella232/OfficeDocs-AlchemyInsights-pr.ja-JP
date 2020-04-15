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
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286268"
---
# <a name="change-strong-password-requirement"></a>強力なパスワードの要件を変更する

既定では、 Microsoft は強力なパスワードを要求します。 

PowerShell で、次のコマンドを使用して、特定のユーザーに対して強力なパスワードを無効にすることができます。<br>
*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*

- [パスワード ポリシーの詳細情報](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [PowerShell で Office 365 に接続する方法](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [PowerShell MsolUser コマンドの詳細情報](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [個別のユーザーのパスワードを無期限に設定する](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)

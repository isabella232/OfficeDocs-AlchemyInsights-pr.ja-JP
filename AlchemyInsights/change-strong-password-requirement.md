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
# <a name="change-strong-password-requirement"></a>強力なパスワードの要件を変更する

Microsoft では、既定で強力なパスワードが必要になります。 

PowerShell を使用すると、次のコマンドを使用して、特定のユーザーの強力なパスワードを無効にすることができます。<br>
*Get-msoluser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [パスワードポリシーの詳細情報](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [PowerShell を使用して Office 365 に接続する方法](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [PowerShell Get-msoluser コマンドの詳細情報](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
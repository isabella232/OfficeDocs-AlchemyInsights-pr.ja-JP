---
title: 強力なパスワードの要件を変更する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 53affd2a347c004e7b21b353c2b3df98bc30a585
ms.sourcegitcommit: a7e5ca472000dfec471950bafd12eee8d7144f74
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741819"
---
# <a name="change-strong-password-requirement"></a>強力なパスワードの要件を変更する

既定では、強力なパスワードが必要です。 

PowerShell を使用すると、次のコマンドを使用して、特定のユーザーの強力なパスワードを無効にすることができます。<br>
*Get-msoluser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [パスワードポリシーの詳細情報](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [PowerShell を使用して O365 に接続する方法](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [PowerShell Get-msoluser コマンドの詳細情報](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
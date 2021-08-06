---
title: ユーザー名を変更できません
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 3088a7b939e7b88319ff688ea94fa71d7fa540787cde31cfd864551113caf149
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020233"
---
# <a name="unable-to-change-username"></a>ユーザー名を変更できません

場合によっては、UPN (UserPrincipalName) の変更がクラウドに反映されないことがあります。 Office 365 ポータルで検証エラーが表示されるか、ユーザー名またはメールアドレスを変更できない可能性があります。 この問題を解決するには、この PowerShell コマンドを使用して、手動で UserPrincipalName を設定します。

**例: ユーザー名を変更する**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

このコマンドは、davidc@contoso.com を davidchew@contoso.com に変更します。

詳細については、[Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)を参照してください。
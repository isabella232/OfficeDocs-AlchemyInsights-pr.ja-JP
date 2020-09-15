---
title: Office のインストールの Teams をアンインストールまたは除外する
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
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658226"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>新規または既存の Office のインストールの Teams をアンインストールまたは除外する

Microsoft Teams は、Microsoft 365 Apps for enterprise、Microsoft 365 Apps for business、Office for Mac の一部として含まれます。

- [Office 展開ツール](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) を使用して、Office の新規インストールから Teams を除外します。
- Windows を実行しているデバイスから Teams を*アンインストール*するには、「[Microsoft Teams をアンインストールする](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)」を参照してください。 複数のターゲット コンピューターまたはユーザーから Microsoft Teams をクリーンアップするには、「[Microsoft Teams の展開のクリーンアップ](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)」を参照してください。
- [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) オプションを使用して、 Microsoft Teams が Office と一緒に自動的にインストールされないようにします。
- *Teams がインストールされる前に*、[PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) オプションを使用して、インストール後に Microsoft Teams が自動的に起動しないようにします。

Office for Mac を使用している場合は、「[Microsoft Teams の Mac へのインストール](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)」を参照してください。
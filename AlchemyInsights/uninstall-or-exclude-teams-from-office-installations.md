---
title: Office インストールから Teams をアンインストールまたは除外する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 6fc5645028c9fb9df2606c0d03b67e87ae15087c
ms.sourcegitcommit: 1e5de64e34e9ba16185b3a895b3152ca61718f4b
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/01/2019
ms.locfileid: "37370708"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>新規または既存の Office のインストールから Teams をアンインストールまたは除外する

Microsoft Teams は、Office 365 ProPlus、Office 365 Business、および Office for Mac の一部として追加されました。

- Office[展開ツール](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus)を使用して、office の新規インストールから Teams を除外します。
- Windows を実行しているデバイスから Teams を*アンインストール*するには、「 [uninstall Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)」を参照してください。 複数のターゲットコンピューターまたはユーザーから Microsoft Teams をクリーンアップするには、「 [Microsoft teams の展開のクリーンアップ](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)」を参照してください。
- [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
)オプションを使用して、Microsoft Teams が Office を使用して自動的にインストールされないようにします。
- *Teams をインストールする前*に[PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)オプションを使用して、Microsoft teams がインストール後に自動的に開始されないようにします。

Office for Mac を使用している場合は、「 [mac での Microsoft Teams のインストール](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)」を参照してください。
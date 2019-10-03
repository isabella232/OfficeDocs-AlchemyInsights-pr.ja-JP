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
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="8ad0e-102">新規または既存の Office のインストールから Teams をアンインストールまたは除外する</span><span class="sxs-lookup"><span data-stu-id="8ad0e-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="8ad0e-103">Microsoft Teams は、Office 365 ProPlus、Office 365 Business、および Office for Mac の一部として追加されました。</span><span class="sxs-lookup"><span data-stu-id="8ad0e-103">Microsoft Teams is now included as part of Office 365 ProPlus, Office 365 Business, and Office for Mac.</span></span>

- <span data-ttu-id="8ad0e-104">Office[展開ツール](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus)を使用して、office の新規インストールから Teams を除外します。</span><span class="sxs-lookup"><span data-stu-id="8ad0e-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="8ad0e-105">Windows を実行しているデバイスから Teams を*アンインストール*するには、「 [uninstall Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ad0e-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="8ad0e-106">複数のターゲットコンピューターまたはユーザーから Microsoft Teams をクリーンアップするには、「 [Microsoft teams の展開のクリーンアップ](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ad0e-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="8ad0e-107">[PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
)オプションを使用して、Microsoft Teams が Office を使用して自動的にインストールされないようにします。</span><span class="sxs-lookup"><span data-stu-id="8ad0e-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="8ad0e-108">*Teams をインストールする前*に[PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)オプションを使用して、Microsoft teams がインストール後に自動的に開始されないようにします。</span><span class="sxs-lookup"><span data-stu-id="8ad0e-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="8ad0e-109">Office for Mac を使用している場合は、「 [mac での Microsoft Teams のインストール](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ad0e-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>
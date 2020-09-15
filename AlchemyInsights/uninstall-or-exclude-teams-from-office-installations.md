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
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="efd21-102">新規または既存の Office のインストールの Teams をアンインストールまたは除外する</span><span class="sxs-lookup"><span data-stu-id="efd21-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="efd21-103">Microsoft Teams は、Microsoft 365 Apps for enterprise、Microsoft 365 Apps for business、Office for Mac の一部として含まれます。</span><span class="sxs-lookup"><span data-stu-id="efd21-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="efd21-104">[Office 展開ツール](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) を使用して、Office の新規インストールから Teams を除外します。</span><span class="sxs-lookup"><span data-stu-id="efd21-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="efd21-105">Windows を実行しているデバイスから Teams を*アンインストール*するには、「[Microsoft Teams をアンインストールする](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efd21-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="efd21-106">複数のターゲット コンピューターまたはユーザーから Microsoft Teams をクリーンアップするには、「[Microsoft Teams の展開のクリーンアップ](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efd21-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="efd21-107">[PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) オプションを使用して、 Microsoft Teams が Office と一緒に自動的にインストールされないようにします。</span><span class="sxs-lookup"><span data-stu-id="efd21-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="efd21-108">*Teams がインストールされる前に*、[PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) オプションを使用して、インストール後に Microsoft Teams が自動的に起動しないようにします。</span><span class="sxs-lookup"><span data-stu-id="efd21-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="efd21-109">Office for Mac を使用している場合は、「[Microsoft Teams の Mac へのインストール](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efd21-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>
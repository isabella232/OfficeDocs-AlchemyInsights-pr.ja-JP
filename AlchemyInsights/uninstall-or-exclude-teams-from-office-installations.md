---
title: Office のインストールの Teams をアンインストールまたは除外する
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
ms.openlocfilehash: c6d5c0233acb8fb71127dcb54c719b71aa1a5bcb
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769812"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="f27df-102">新規または既存の Office のインストールの Teams をアンインストールまたは除外する</span><span class="sxs-lookup"><span data-stu-id="f27df-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="f27df-103">Microsoft Teams は、Office 365 ProPlus、Office 365 Business、および Office for Mac の一部として含まれています。</span><span class="sxs-lookup"><span data-stu-id="f27df-103">Microsoft Teams is now included as part of new installations of Office 365 ProPlus, Office 365 Business, and Office for Mac.</span></span>

- <span data-ttu-id="f27df-104">[Office 展開ツール](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) を使用して、Office の新規インストールから Teams を除外します。</span><span class="sxs-lookup"><span data-stu-id="f27df-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="f27df-105">Windows を実行しているデバイスから Teams を*アンインストール*するには、「[Microsoft Teams をアンインストールする](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f27df-105">To *uninstall Teams* from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="f27df-106">複数のターゲット コンピューターまたはユーザーから Microsoft Teams をクリーンアップするには、「[Microsoft Teams の展開のクリーンアップ](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f27df-106">To cleanup Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="f27df-107">[PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) オプションを使用して、 Microsoft Teams が Office と一緒に自動的にインストールされないようにします。</span><span class="sxs-lookup"><span data-stu-id="f27df-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="f27df-108">*Teams がインストールされる前に*、[PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) オプションを使用して、インストール後に Microsoft Teams が自動的に起動しないようにします。</span><span class="sxs-lookup"><span data-stu-id="f27df-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="f27df-109">Office for Mac を使用している場合は、「[Microsoft Teams の Mac へのインストール](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f27df-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>
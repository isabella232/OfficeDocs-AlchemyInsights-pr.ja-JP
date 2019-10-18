---
title: Teams をスタンドアロンとして、または新規または既存の Offic eインストールで展開する
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/01/2019
ms.locfileid: "36180402"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a><span data-ttu-id="f4f19-102">Teams をスタンドアロンとして、または新規または既存の Offic eインストールで展開する</span><span class="sxs-lookup"><span data-stu-id="f4f19-102">Deploying Teams as standalone or with new or existing Office installations</span></span>

<span data-ttu-id="f4f19-103">Microsoft Teams は、Office 365 ProPlus、Office 365 Business、および Office for Mac の***新規インストール***の一部として含まれるようになりました。</span><span class="sxs-lookup"><span data-stu-id="f4f19-103">Microsoft Teams is now included as part of ***new installations*** of Office 365 ProPlus, Office 365 Business, and Office for Mac.</span></span> <span data-ttu-id="f4f19-104">詳細については、「[Microsoft Teams は、いつ Office の新規インストールに含まれるようになりますか?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4f19-104">For more information, see [When will Microsoft Teams start being included with new installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)</span></span>

<span data-ttu-id="f4f19-105">さらに、月次チャネルのバージョン 1906 以降、Windows を実行しているデバイスで既存のインストールを最新バージョンに更新する際に、Teams が***既存の Office 365 ProPlus (および Office 365 Business) インストールに追加***されます。</span><span class="sxs-lookup"><span data-stu-id="f4f19-105">Additionally, starting with Version 1906 in Monthly Channel, Teams will be ***added to existing installations*** of Office 365 ProPlus (and Office 365 Business) on devices running Windows when you update your existing installation to the latest version.</span></span> <span data-ttu-id="f4f19-106">詳細については、「[既存の Office のインストールについて](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4f19-106">For more information, see [What about existing installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)</span></span>

> [!NOTE]
> <span data-ttu-id="f4f19-107">この展開スケジュールを待たない場合は、[次の手順に従って](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) 、ユーザーに Teams をスタンドアロンとして展開することができます。または、ユーザーが  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) から自分で Teams をインストールすることもできます。</span><span class="sxs-lookup"><span data-stu-id="f4f19-107">If you don't want to wait for this rollout schedule, you can deploy Teams as standalone for your users by [following these instructions](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) or you can have your users install Teams for themselves from [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).</span></span>

<span data-ttu-id="f4f19-108">組織が Teams を展開する準備ができていない場合、Office の[新規](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus)または[既存](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams)のインストールから ***Teams を除外***する手順があります。</span><span class="sxs-lookup"><span data-stu-id="f4f19-108">If your organization isn't ready to deploy Teams, we have the steps you can take to ***exclude Teams*** from [new](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) or [existing](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installations of Office.</span></span> <span data-ttu-id="f4f19-109">Teams をインストールする必要があるが、インストール後、ユーザーに対して Teams が自動的に起動されないようにする場合は、「[インストール後に Microsoft Teams の自動起動を回避する](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4f19-109">If you want Teams to be installed, but don't want Teams to start automatically for the user after it's installed, see [Prevent Microsoft Teams from starting automatically after installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).</span></span>

<span data-ttu-id="f4f19-110">Windows を実行しているデバイスから ***Teams をアンインストール***するには、「[Microsoft Teams のアンインストール](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4f19-110">To ***uninstall Teams*** from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="f4f19-111">複数のターゲット コンピューターまたはユーザーから Microsoft Teams をクリーンアップするには、「[Microsoft Teams の展開のクリーンアップ](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4f19-111">To cleanup Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>

<span data-ttu-id="f4f19-112">共有コンピューター、リモート デスクトップ サービス (RDS) または仮想デスクトップ インフラストラクチャ (VDI) を使用している場合は、「[Microsoft Teams での共有コンピューターおよび VDI 環境](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4f19-112">If you're using shared computers, Remote Desktop Services (RDS), or Virtual Desktop Infrastructure (VDI), see [Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).</span></span>

<span data-ttu-id="f4f19-113">Office for Mac を使用している場合は、「[Microsoft Teams の Mac へのインストール](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4f19-113">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>

> [!NOTE]
> <span data-ttu-id="f4f19-114">インストール後の Teams は、約 2 週間ごとに新しい機能と品質の更新プログラムによって[自動的に更新](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)されます。</span><span class="sxs-lookup"><span data-stu-id="f4f19-114">After Teams is installed, it's [automatically updated](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) approximately every two weeks with new features and quality updates.</span></span> 
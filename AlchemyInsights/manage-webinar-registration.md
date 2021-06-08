---
title: ウェビナー登録の管理
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798649"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="e280c-102">ウェビナー登録の管理</span><span class="sxs-lookup"><span data-stu-id="e280c-102">Manage webinar registration</span></span>

<span data-ttu-id="e280c-103">Teams Powershell コマンドを使用して、Teams ウェビナーに登録できるユーザーを管理します。</span><span class="sxs-lookup"><span data-stu-id="e280c-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="e280c-104">Teams PowerShell をインストールするには、「[Teams PowerShell](/microsoftteams/teams-powershell-install)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e280c-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="e280c-105">既定では、*WhoCanRegister* が有効になっており、[**Everyone**] に設定されています。</span><span class="sxs-lookup"><span data-stu-id="e280c-105">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> 

<span data-ttu-id="e280c-106">会議出席依頼にすべてのユーザー の登録を許可するオプションが表示されない場合は、*WhoCanRegister* 設定を [すべてのユーザー] に再実行し、24 時間待ちます。</span><span class="sxs-lookup"><span data-stu-id="e280c-106">If you don't see the option to allow registration for Everyone in the meeting invitation, rerun setting *WhoCanRegister* to Everyone and wait 24 hours.</span></span> <span data-ttu-id="e280c-107">*WhoCanRegister* を再実行するには、Powershell コマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="e280c-107">To rerun *WhoCanRegister*, use the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="e280c-108">**注**: 会議の設定で匿名参加がオフになっている場合、匿名ユーザーはウェビナーに参加できません。</span><span class="sxs-lookup"><span data-stu-id="e280c-108">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="e280c-109">この設定の詳細と有効化については、「[Microsoft Teams で会議設定を管理する](/microsoftteams/meeting-settings-in-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e280c-109">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="e280c-110">会議の登録を無効にする場合は、*AllowMeetingRegistration* を **False** に設定します。</span><span class="sxs-lookup"><span data-stu-id="e280c-110">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="e280c-111">ウェビナーに登録できるユーザーの構成の詳細については、「[ウェビナーに登録できるユーザーを構成する](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)」 を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e280c-111">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="e280c-112">Microsoft Lists の設定の詳細については、「 [Microsoft Lists のコントロール設定」](/sharepoint/control-lists)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e280c-112">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>

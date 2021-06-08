---
title: Teams のウェビナーを有効にする
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794246"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="2cd98-102">Teams のウェビナーを有効にする</span><span class="sxs-lookup"><span data-stu-id="2cd98-102">Enable Teams Webinars</span></span>

<span data-ttu-id="2cd98-103">ウェビナーは既定で有効になっています。</span><span class="sxs-lookup"><span data-stu-id="2cd98-103">Webinars are enabled by default.</span></span> <span data-ttu-id="2cd98-104">Teams Powershell コマンドを使用して、スケジュールを行ってTeams ウェビナーに登録できるユーザーを管理します。</span><span class="sxs-lookup"><span data-stu-id="2cd98-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="2cd98-105">会議を作成できるすべてのユーザーは、ウェビナー会議を作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="2cd98-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="2cd98-106">Teams ウェビナーをスケジュールできるユーザーを管理する場合は、*AllowMeetingRegistration* を使用します。</span><span class="sxs-lookup"><span data-stu-id="2cd98-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="2cd98-107">既定では、*WhoCanRegister* が有効になっており、[**Everyone**] に設定されています。</span><span class="sxs-lookup"><span data-stu-id="2cd98-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="2cd98-108">会議の登録を無効にする場合は、*AllowMeetingRegistration* を **False** に設定します。</span><span class="sxs-lookup"><span data-stu-id="2cd98-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="2cd98-109">これらの設定を変更するには、[Teams PowerShell](/microsoftteams/teams-powershell-install) をインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="2cd98-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="2cd98-110">また、会議ポリシーが Teams ウェビナーに適用されます。</span><span class="sxs-lookup"><span data-stu-id="2cd98-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="2cd98-111">たとえば、会議の設定で匿名参加がオフになっている場合、匿名ユーザーはウェビナーに参加できません。</span><span class="sxs-lookup"><span data-stu-id="2cd98-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="2cd98-112">ウェビナーに登録できるユーザーの構成の詳細については、「[ウェビナーに登録できるユーザーを構成する](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)」 を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2cd98-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="2cd98-113">Microsoft Lists の設定の詳細については、「 [Microsoft Lists のコントロール設定」](/sharepoint/control-lists)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2cd98-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
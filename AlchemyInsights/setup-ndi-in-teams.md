---
title: NDI テクノロジを有効にする
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935224"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="32f34-102">NDI テクノロジを有効にする</span><span class="sxs-lookup"><span data-stu-id="32f34-102">Turn on NDI technology</span></span>

<span data-ttu-id="32f34-103">NDI テクノロジでは、ユーザーに対して次の 2 つの手順を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="32f34-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="32f34-104">テナント管理者が CsTeamsMeetingPolicy で「AllowNDIStreaming」プロパティを有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="32f34-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="32f34-105">この変更が設定された後、エンド ユーザーは、**[設定]、[アクセス許可]** の順に移動して特定のクライアントの NDI® テクノロジを有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="32f34-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="32f34-106">詳細については、「[Microsoft Teams で NDI テクノロジを使用する](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32f34-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>

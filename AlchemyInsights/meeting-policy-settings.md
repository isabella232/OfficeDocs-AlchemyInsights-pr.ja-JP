---
title: 会議ポリシーの設定
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627579"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="25f4d-102">Microsoft Teams で会議ポリシーを管理する</span><span class="sxs-lookup"><span data-stu-id="25f4d-102">Manage meeting policies in Teams</span></span>

<span data-ttu-id="25f4d-103">会議ポリシーは、組織内のユーザーによってスケジュールされた会議への参加者が利用できる機能を制御するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="25f4d-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="25f4d-104">会議ポリシーの一部の機能は、Teams 管理センターにまだ実装されていない場合があります (これらはドキュメントに "近日公開" としてラベル付けされています)。</span><span class="sxs-lookup"><span data-stu-id="25f4d-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="25f4d-105">この場合、もしくは Microsoft Teams 管理センターで "今すぐポリシーを更新することはできませんが、後でもう一度試してください" などのエラーが表示される場合には、PowerShell を使用して Teams 会議ポリシーを作成または変更することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="25f4d-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="25f4d-106">会議ポリシーの詳細については、以下のリソースをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="25f4d-106">For more information about BranchCache, see the following resources:</span></span>

- <span data-ttu-id="25f4d-107">ポリシーの作成、変更、およびポリシーへのユーザーの割り当ての詳細については、「[Teams での会議ポリシーを管理する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25f4d-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="25f4d-108">PowerShell コマンドレットを使用してポリシーを変更するには、「[Teams での PowerShell の概要](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25f4d-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="25f4d-109">Teams の会議ポリシーには、[Skype for Business PowerShell モジュール](https://www.microsoft.com/download/details.aspx?id=39366)を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="25f4d-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="25f4d-110">詳細については、[\*-CsTeamsMeetingPolicy コマンドレットのドキュメント](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25f4d-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="25f4d-111">**注:** ポリシーの変更がユーザーに反映されるまで最大 24 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="25f4d-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="25f4d-112">新しく作成されたポリシーをすぐに変更できない場合があります。4 時間待ってから、新しく作成されたポリシーを再度変更してみてください。</span><span class="sxs-lookup"><span data-stu-id="25f4d-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="25f4d-113">それでも問題が解決しない場合には、PowerShell を試してみてください。</span><span class="sxs-lookup"><span data-stu-id="25f4d-113">If you're still having problems, try PowerShell.</span></span>  
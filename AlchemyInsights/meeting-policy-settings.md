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
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/02/2019
ms.locfileid: "37380100"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="86ea5-102">Microsoft Teams での会議ポリシーの管理</span><span class="sxs-lookup"><span data-stu-id="86ea5-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="86ea5-103">会議ポリシーは、組織内のユーザーによってスケジュールされた会議の会議参加者が使用できる機能を制御するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="86ea5-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="86ea5-104">会議ポリシーの一部の機能は、Teams 管理センターには実装されていない場合があります (ドキュメントの「近日中」というラベルが付いています)。</span><span class="sxs-lookup"><span data-stu-id="86ea5-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="86ea5-105">この場合、または Microsoft Teams の管理センターで "ポリシーを今すぐには更新できません。後でもう一度実行してください" のようなエラーが表示される場合は、PowerShell を使用して Teams の会議ポリシーを作成または変更することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="86ea5-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="86ea5-106">会議ポリシーの詳細については、次のリソースを参照してください。</span><span class="sxs-lookup"><span data-stu-id="86ea5-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="86ea5-107">ポリシーの作成、変更、およびポリシーへのユーザーの割り当てについては、「 [Teams での会議ポリシーの管理](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86ea5-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="86ea5-108">PowerShell コマンドレットを使用してポリシーを変更するには、「 [Teams powershell の概要](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86ea5-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="86ea5-109">Teams の会議ポリシーには、 [Skype For Business PowerShell モジュール](https://www.microsoft.com/download/details.aspx?id=39366)を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="86ea5-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="86ea5-110">詳細については、 [CsTeamsMeetingPolicy コマンドレットのドキュメント](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86ea5-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="86ea5-111">**注:** ユーザーがポリシーの変更を有効にするには、最大24時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="86ea5-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="86ea5-112">新しく作成したポリシーをすぐに変更できない場合があります。4時間待ってから、新しく作成したポリシーをもう一度変更します。</span><span class="sxs-lookup"><span data-stu-id="86ea5-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="86ea5-113">それでも問題が解決しない場合は、PowerShell をお試しください。</span><span class="sxs-lookup"><span data-stu-id="86ea5-113">If you're still having problems, try PowerShell.</span></span>  
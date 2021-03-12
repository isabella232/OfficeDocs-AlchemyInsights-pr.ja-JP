---
title: 会議ポリシーの設定
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704611"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="e8e90-102">Microsoft Teams で会議ポリシーを管理する</span><span class="sxs-lookup"><span data-stu-id="e8e90-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="e8e90-103">**注: ポリシーの変更がユーザーに反映されるまで最大 24 時間かかる場合があります。**</span><span class="sxs-lookup"><span data-stu-id="e8e90-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="e8e90-104">新しく作成されたポリシーをすぐに変更できない場合があります。4 時間待ってから、新しく作成されたポリシーを再度変更してみてください。</span><span class="sxs-lookup"><span data-stu-id="e8e90-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="e8e90-105">会議ポリシーは、組織内のユーザーによってスケジュールされた会議への参加者が利用できる機能を制御するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="e8e90-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="e8e90-106">会議ポリシーの一部の機能は、Teams 管理センターにまだ実装されていない場合があります (これらはドキュメントに "近日公開" としてラベル付けされています)。</span><span class="sxs-lookup"><span data-stu-id="e8e90-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="e8e90-107">この場合、もしくは Microsoft Teams 管理センターで "今すぐポリシーを更新することはできませんが、後でもう一度試してください" などのエラーが表示される場合には、PowerShell を使用して Teams 会議ポリシーを作成または変更することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e8e90-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="e8e90-108">会議ポリシーの詳細については、以下のリソースをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e8e90-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="e8e90-109">ポリシーの作成、変更、およびポリシーへのユーザーの割り当ての詳細については、「[Teams での会議ポリシーを管理する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8e90-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="e8e90-110">PowerShell コマンドレットを使用してポリシーを変更するには、「[Teams での PowerShell の概要](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8e90-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="e8e90-111">Teams の会議ポリシーには、[Skype for Business PowerShell モジュール](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector)を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8e90-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="e8e90-112">詳細については、[\*-CsTeamsMeetingPolicy コマンドレットのドキュメント](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8e90-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>


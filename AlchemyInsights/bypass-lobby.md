---
title: ロビーのバイパス
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820039"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="06bb6-102">Teams でロビーの設定と参加レベルを制御する</span><span class="sxs-lookup"><span data-stu-id="06bb6-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="06bb6-103">ダイヤルイン ユーザー、外部ユーザー、匿名ユーザーを含むすべてのユーザーが **ロビーをバイパス** できるようにするには、PowerShell を使用してこれを行えます。</span><span class="sxs-lookup"><span data-stu-id="06bb6-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="06bb6-104">組織のグローバル会議ポリシーを変更する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06bb6-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="06bb6-105">現在、このコマンドレットでは Skype for Business PowerShell モジュールを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="06bb6-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="06bb6-106">このコマンドレットを使用するための設定方法については、「[PowerShell によるポリシーの管理](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06bb6-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="06bb6-107">ポリシーの設定が完了したら、ポリシーをユーザーに適用する必要があります。ただし、グローバル ポリシーを変更した場合は、ポリシーは自動的にユーザーに適用されます。</span><span class="sxs-lookup"><span data-stu-id="06bb6-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="06bb6-108">ポリシーを変更した場合、ポリシーが有効になるまで少なくとも **4 時間、最大で 24 時間** 待つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="06bb6-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="06bb6-109">これらの変更を行う前に、下のドキュメントをよく確認し、許可される内容について正確に理解するようにします。</span><span class="sxs-lookup"><span data-stu-id="06bb6-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="06bb6-110">Teams の会議ロビー ポリシーの制御の説明</span><span class="sxs-lookup"><span data-stu-id="06bb6-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="06bb6-111">これらの設定では、会議への入室が許可されるまでロビーで待機する必要がある会議参加者およびそれらの参加者に許可する会議への参加レベルが制御されます。</span><span class="sxs-lookup"><span data-stu-id="06bb6-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="06bb6-112">PowerShell を使用することで、Teams 管理センターでまだ実装されていない ("準備中" というラベルが付いている) 会議ポリシーの設定を更新できます。 </span><span class="sxs-lookup"><span data-stu-id="06bb6-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="06bb6-113">ロビーをバイパスすることをすべてのユーザーに許可するための PowerShell コマンドレットの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06bb6-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="06bb6-114">[[ユーザーの参加を自動的に許可する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)] は開催者単位のポリシーで、ユーザーは会議に直接参加するのか、認証されたユーザーにより入室が許可されるまでロビーで待機するのかを制御します。</span><span class="sxs-lookup"><span data-stu-id="06bb6-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="06bb6-115">[[匿名ユーザーに会議の開始を許可する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)] は開催者単位のポリシーで、認証された組織のユーザーが参加していない場合でも、B2B ユーザーおよびフェデレーション ユーザーなどの匿名ユーザーがユーザーの会議に参加できるかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="06bb6-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="06bb6-116">[[ダイヤルイン ユーザーによるロビーのバイパスを許可する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)] (**近日公開予定**) は開催者単位のポリシーで、電話を使用してダイヤルインするユーザーは会議に直接参加するのか、[**ユーザーの参加を自動的に許可する**] の設定に関わらずロビーで待機するのかを制御します。</span><span class="sxs-lookup"><span data-stu-id="06bb6-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="06bb6-117">[[開催者によるロビーの設定の上書きを許可する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)] (**近日公開予定**) は開催者単位のポリシーで、管理者が新しい会議のスケジュール時に設定した [**ユーザーの参加を自動的に許可する**] または [**ダイヤルイン ユーザーによるロビーのバイパスを許可する**] のロビー設定を会議開催者がオーバーライドできるかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="06bb6-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="06bb6-118">**注:** Microsoft Teams の会議ポリシーの完全な概要については、「[Teams で会議ポリシーを管理する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06bb6-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>

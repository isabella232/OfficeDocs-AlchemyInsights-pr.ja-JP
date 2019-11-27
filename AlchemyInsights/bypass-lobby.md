---
title: ロビーのバイパス
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768445"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="65d70-102">ロビーの設定と参加レベルを制御する</span><span class="sxs-lookup"><span data-stu-id="65d70-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="65d70-103">ダイヤルイン ユーザー、外部ユーザー、匿名ユーザーを含むすべてのユーザーが Microsoft Teams のロビーをバイパスできるようにするには、PowerShell を使用してこれを行えます。</span><span class="sxs-lookup"><span data-stu-id="65d70-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="65d70-104">組織のグローバル会議ポリシーを変更する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="65d70-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="65d70-105">現在、このコマンドレットでは Skype for Business PowerShell モジュールを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="65d70-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="65d70-106">このコマンドレットを使用するための設定方法については、「[PowerShell によるポリシーの管理](https://docs.microsoft.com/ja-JP/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65d70-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/ja-JP/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="65d70-107">新しいポリシーをセットアップすることができます。そのポリシーはユーザーに適用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="65d70-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="65d70-108">グローバル ポリシーを変更した場合、変更されたポリシーは自動的にユーザーに適用されます。</span><span class="sxs-lookup"><span data-stu-id="65d70-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="65d70-109">ポリシーを変更した場合、ポリシーが有効になるまで少なくとも 4 時間、最大で 24 時間待つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="65d70-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="65d70-110">これらの変更を行う前に、下のドキュメントをよく確認し、許可される内容について正確に理解するようにします。</span><span class="sxs-lookup"><span data-stu-id="65d70-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="65d70-111">Teams の会議ロビー ポリシーの制御の説明</span><span class="sxs-lookup"><span data-stu-id="65d70-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="65d70-112">[[ユーザーの参加を自動的に許可する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)] は開催者単位のポリシーで、ユーザーは会議に直接参加するのか、認証されたユーザーにより入室が許可されるまでロビーで待機するのかを制御します。</span><span class="sxs-lookup"><span data-stu-id="65d70-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="65d70-113">[[匿名ユーザーに会議の開始を許可する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)] は開催者単位のポリシーで、認証された組織のユーザーが参加していない場合でも、B2B ユーザーおよびフェデレーション ユーザーなどの匿名ユーザーがユーザーの会議に参加できるかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="65d70-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="65d70-114">[[ダイヤルイン ユーザーによるロビーのバイパスを許可する](https://docs.microsoft.com/ja-JP/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)] (**近日公開予定**) は開催者単位のポリシーで、電話を使用してダイヤルインするユーザーは会議に直接参加するのか、[**ユーザーの参加を自動的に許可する**] の設定に関わらずロビーで待機するのかを制御します。</span><span class="sxs-lookup"><span data-stu-id="65d70-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/ja-JP/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="65d70-115">[[開催者によるロビーの設定の上書きを許可する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)] (**近日公開予定**) は開催者単位のポリシーで、管理者が新しい会議のスケジュール時に設定した [**ユーザーの参加を自動的に許可する**] または [**ダイヤルイン ユーザーによるロビーのバイパスを許可する**] のロビー設定を会議開催者がオーバーライドできるかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="65d70-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="65d70-116">**注:** Microsoft Teams の会議ポリシーの完全な概要については、「[Teams で会議ポリシーを管理する](https://docs.microsoft.com/ja-JP/microsoftteams/meeting-policies-in-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65d70-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/ja-JP/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>

---
title: バイパスロビー
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
ms.openlocfilehash: 729fc5d4213acbbdf74a9d07adacb42b34170717
ms.sourcegitcommit: ffbeb72c9199ab4ebcb0f1ad443ed3e2f4950efc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637782"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="5cbed-102">ロビーの設定と参加レベルの制御</span><span class="sxs-lookup"><span data-stu-id="5cbed-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="5cbed-103">ダイヤルイン、外部、匿名の各ユーザーを含むすべてのユーザーがロビーをバイパスできるようにする場合は、PowerShell を使用して実行できます。</span><span class="sxs-lookup"><span data-stu-id="5cbed-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="5cbed-104">組織のグローバル会議ポリシーを変更する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5cbed-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="5cbed-105">現在、このコマンドレットでは、Skype for Business PowerShell モジュールを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5cbed-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="5cbed-106">このコマンドレットを使用するには、PowerShell を使用してポリシーを管理することをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="5cbed-106">To get setup to use this cmdlet, check out Managing policies via PowerShell.</span></span>

<span data-ttu-id="5cbed-107">新しいポリシーをセットアップして、ユーザーに適用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5cbed-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="5cbed-108">グローバルポリシーを変更すると、ユーザーに自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5cbed-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="5cbed-109">ポリシーを変更する場合は、ポリシーが有効になるまで、少なくとも4時間、最大24時間待機する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5cbed-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="5cbed-110">このような変更を行う前に、次のドキュメントを必ず確認してください。</span><span class="sxs-lookup"><span data-stu-id="5cbed-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="5cbed-111">Teams 会議ロビーポリシーコントロールについて</span><span class="sxs-lookup"><span data-stu-id="5cbed-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="5cbed-112">[[ユーザーに自動的に](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)許可するのは開催者ごとのポリシーで、ユーザーが会議に直接参加するか、認証されたユーザーによって許可されるまでロビーで待機するかを制御します。</span><span class="sxs-lookup"><span data-stu-id="5cbed-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="5cbed-113">[[匿名ユーザーによる会議の開始を許可](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)する] は、組織の承認されたユーザーが参加していない場合に、B2B ユーザーやフェデレーションユーザーを含む匿名ユーザーがユーザーの会議に参加できるかどうかを制御する、開催者ごとのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="5cbed-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="5cbed-114">[[ダイヤルインユーザーがロビーをバイパスすることを許可する](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)] (**近日**中に) は、電話でダイヤルインするユーザーが、**自動的にユーザー**の設定に関係なく、ミーティングに直接参加するか、またはロビーで待機するかを制御する開催者ごとのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="5cbed-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="5cbed-115">[[開催者にロビーの設定を上書きすることを許可](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)する] (**近日**) は開催者ごとのポリシーで、会議の開催者が**自動的にユーザー**を許可し、ダイヤルインを**許可するために管理者が設定したロビー設定を上書きできるかどうかを制御します。ユーザー**が新しい会議をスケジュールするときに、ロビーをバイパスする。</span><span class="sxs-lookup"><span data-stu-id="5cbed-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="5cbed-116">**注:** Microsoft Teams の会議ポリシーの完全な概要については、「 [teams での会議ポリシーの管理](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5cbed-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>

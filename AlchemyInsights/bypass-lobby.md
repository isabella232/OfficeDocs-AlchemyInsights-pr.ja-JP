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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/02/2019
ms.locfileid: "37380105"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="953a3-102">ロビーの設定と参加レベルの制御</span><span class="sxs-lookup"><span data-stu-id="953a3-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="953a3-103">これらの設定は、参加者が会議に参加する前にロビーで待機する会議の参加者と、会議で許可されている参加レベルを制御します。</span><span class="sxs-lookup"><span data-stu-id="953a3-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="953a3-104">Powershell を使用すると、Teams の管理センターで、まだ実装されていない (「近いうちに」というラベルの) ミーティングポリシー設定を更新できます。</span><span class="sxs-lookup"><span data-stu-id="953a3-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="953a3-105">すべてのユーザーがロビーをバイパスできるようにする PowerShell コマンドレットの例については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="953a3-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="953a3-106">[[ユーザーに自動的に](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)許可するのは開催者ごとのポリシーで、ユーザーが会議に直接参加するか、認証されたユーザーによって許可されるまでロビーで待機するかを制御します。</span><span class="sxs-lookup"><span data-stu-id="953a3-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="953a3-107">[[匿名ユーザーによる会議の開始を許可](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)する] は、組織の承認されたユーザーが参加していない場合に、B2B ユーザーやフェデレーションユーザーを含む匿名ユーザーがユーザーの会議に参加できるかどうかを制御する、開催者ごとのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="953a3-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="953a3-108">[[ダイヤルインユーザーがロビーをバイパスすることを許可する](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)] (**近日**中に) は、電話でダイヤルインするユーザーが、**自動的にユーザー**の設定に関係なく、ミーティングに直接参加するか、またはロビーで待機するかを制御する開催者ごとのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="953a3-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="953a3-109">[[開催者にロビーの設定を上書きすることを許可](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)する] (**近日**) は開催者ごとのポリシーで、会議の開催者が**自動的にユーザー**を許可し、ダイヤルインを**許可するために管理者が設定したロビー設定を上書きできるかどうかを制御します。ユーザー**が新しい会議をスケジュールするときに、ロビーをバイパスする。</span><span class="sxs-lookup"><span data-stu-id="953a3-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="953a3-110">**注:** Microsoft Teams の会議ポリシーの完全な概要については、「 [teams での会議ポリシーの管理](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="953a3-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="953a3-111">**PowerShell の例**</span><span class="sxs-lookup"><span data-stu-id="953a3-111">**PowerShell example**</span></span>

<span data-ttu-id="953a3-112">外部または匿名ユーザーを含むすべてのユーザーがロビーをバイパスできるようにする場合は、PowerShell を使用してこのタスクを実行することもできます。</span><span class="sxs-lookup"><span data-stu-id="953a3-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="953a3-113">ここでは、組織のグローバル会議ポリシーを変更する例を示します。</span><span class="sxs-lookup"><span data-stu-id="953a3-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="953a3-114">(この変更を行う前に、上記のドキュメントを必ずご確認ください)。</span><span class="sxs-lookup"><span data-stu-id="953a3-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="953a3-115">CsTeamsMeetingPolicy-Identity Global-AutoAdmittedUsers 「Everyone」-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="953a3-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="953a3-116">詳細については、「 [CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="953a3-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>

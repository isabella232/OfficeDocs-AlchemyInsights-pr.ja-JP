---
title: ユーザーによる会議の記録をブロックする
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038258"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="b477a-102">ユーザーによる会議の記録をブロックする</span><span class="sxs-lookup"><span data-stu-id="b477a-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="b477a-103">特定のユーザーによるチーム会議の記録を **防止またはブロック** する必要がある場合は、Teams 会議ポリシー設定を使用して行うことができます。</span><span class="sxs-lookup"><span data-stu-id="b477a-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="b477a-104">Microsoft Teams 管理センターを使用する場合は、そのユーザーに割り当てられている会議ポリシーの **[Allow cloud recording](クラウド レコーディングを許可する)** 設定をオフにします。</span><span class="sxs-lookup"><span data-stu-id="b477a-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="b477a-105">詳細については、「[Teams での会議ポリシーを管理する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b477a-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="b477a-106">特定のユーザーがTeams 会議の記録を許可されているかどうかを検証するには、サポート診断を使用します。</span><span class="sxs-lookup"><span data-stu-id="b477a-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="b477a-107">新しいサポートクエリを実行し、**Diag: Meeting Recording** と入力します - 診断は、指定されたユーザーのポリシー設定をチェックし、そのポリシー設定を決定します。</span><span class="sxs-lookup"><span data-stu-id="b477a-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="b477a-108">新しいポリシー設定が有効になるまでに数時間かかる場合があるため、変更を加えたばかりの場合は、数時間待ってから診断を再度実行してください。</span><span class="sxs-lookup"><span data-stu-id="b477a-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="b477a-109">詳細については、「[クラウド レコーディングを開始または停止する](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="b477a-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>

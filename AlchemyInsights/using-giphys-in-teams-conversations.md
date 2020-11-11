---
title: Teams 会話での Giphy の使用
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
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982627"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="6cba9-102">Teams 会話での Giphy の使用</span><span class="sxs-lookup"><span data-stu-id="6cba9-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="6cba9-103">Teams チャットの Giphy アクセスは、既定で有効になっています。</span><span class="sxs-lookup"><span data-stu-id="6cba9-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="6cba9-104">管理者は、 [メッセージング ポリシーを設定](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings)し、 **[会話で Giphy を使用する]** が **[オン]** であることを確認することで、ユーザーが Giphy を使用できるかどうかを制御できます。</span><span class="sxs-lookup"><span data-stu-id="6cba9-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="6cba9-105">GIF が Teams 会話で期待どおりに動作しない場合は、次のことを確認します。</span><span class="sxs-lookup"><span data-stu-id="6cba9-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="6cba9-106">[メッセージング ポリシー](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams)で Giphy を許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6cba9-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="6cba9-107">PowerShell コマンドレットを使用して確認するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="6cba9-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="6cba9-108">[PowerShell を使用して Teams を管理](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="6cba9-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="6cba9-109">PowerShell コマンド [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) を実行して、 **AllowGiphy** が **TRUE** に設定されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="6cba9-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="6cba9-110">**AllowGiphy** が **FALSE** に設定されている場合、次の PowerShell コマンド [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps) を実行します。</span><span class="sxs-lookup"><span data-stu-id="6cba9-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="6cba9-111">[オプションの接続エクスペリエンス](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences)を使用するように設定して、Giphy URL にアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="6cba9-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="6cba9-112">テナントに複数の Teams メッセージング ポリシーが構成されている場合、PowerShell コマンド [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy を使用して影響を受けるユーザーに割り当てられたポリシーの ID を確認することができます。</span><span class="sxs-lookup"><span data-stu-id="6cba9-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>

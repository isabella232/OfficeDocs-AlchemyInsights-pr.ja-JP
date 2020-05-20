---
title: プライベート チャネル
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005443"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="d4e07-102">Microsoft Teams のプライベート チャネル</span><span class="sxs-lookup"><span data-stu-id="d4e07-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="d4e07-103">プライベート チャネルは、Microsoft Teams の新機能です。</span><span class="sxs-lookup"><span data-stu-id="d4e07-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="d4e07-104">プライベート チャネルは、標準チャネルから変換することも、その逆にすることもできません。</span><span class="sxs-lookup"><span data-stu-id="d4e07-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="d4e07-105">[プライベート チャネルの作成とメンバーシップ](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership)、[プライベート チャネル SharePoint サイト](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)などのプライベート チャネルの詳細については、「[Microsoft Teams のプライベート チャネル](https://docs.microsoft.com/MicrosoftTeams/private-channels)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4e07-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="d4e07-106">**注:** プライベート チャネル メッセージの保持の構成はまだサポートされていないため、保持ポリシーが有効になっているテナントでは、既定でプライベート チャネルが有効になりません。</span><span class="sxs-lookup"><span data-stu-id="d4e07-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="d4e07-107">プライベート チャネルは、Teams 管理センターで有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d4e07-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="d4e07-108">また、プライベート チャネル メッセージの保持はサポートされていませんが、プライベート チャネルで共有されているファイルの保持はサポートされます。</span><span class="sxs-lookup"><span data-stu-id="d4e07-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="d4e07-109">**新しいチーム所有者が必要ですか?**</span><span class="sxs-lookup"><span data-stu-id="d4e07-109">**Need a new team owner?**</span></span>

<span data-ttu-id="d4e07-110">プライベート チャネルの所有者が退職した場合は、Teams Powershell を使用して新しいチーム所有者を追加することができます。</span><span class="sxs-lookup"><span data-stu-id="d4e07-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="d4e07-111">[ここに](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6)移動して、Teams Powershell をインストールします。</span><span class="sxs-lookup"><span data-stu-id="d4e07-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="d4e07-112">必要なコマンドレットを以下に示します。</span><span class="sxs-lookup"><span data-stu-id="d4e07-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="d4e07-113">Teams Powershell の詳細については、「[Teams での PowerShell の概要](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4e07-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>

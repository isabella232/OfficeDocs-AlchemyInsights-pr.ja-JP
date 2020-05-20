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
# <a name="private-channels-in-microsoft-teams"></a>Microsoft Teams のプライベート チャネル

プライベート チャネルは、Microsoft Teams の新機能です。 プライベート チャネルは、標準チャネルから変換することも、その逆にすることもできません。

[プライベート チャネルの作成とメンバーシップ](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership)、[プライベート チャネル SharePoint サイト](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)などのプライベート チャネルの詳細については、「[Microsoft Teams のプライベート チャネル](https://docs.microsoft.com/MicrosoftTeams/private-channels)」を参照してください。 

**注:** プライベート チャネル メッセージの保持の構成はまだサポートされていないため、保持ポリシーが有効になっているテナントでは、既定でプライベート チャネルが有効になりません。 プライベート チャネルは、Teams 管理センターで有効にすることができます。 また、プライベート チャネル メッセージの保持はサポートされていませんが、プライベート チャネルで共有されているファイルの保持はサポートされます。

**新しいチーム所有者が必要ですか?**

プライベート チャネルの所有者が退職した場合は、Teams Powershell を使用して新しいチーム所有者を追加することができます。


- [ここに](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6)移動して、Teams Powershell をインストールします。

必要なコマンドレットを以下に示します。

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Teams Powershell の詳細については、「[Teams での PowerShell の概要](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)」を参照してください。

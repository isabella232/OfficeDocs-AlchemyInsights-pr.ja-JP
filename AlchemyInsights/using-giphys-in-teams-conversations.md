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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104313"
---
# <a name="using-giphys-in-teams-conversations"></a>Teams 会話での Giphy の使用

Teams チャットの Giphy アクセスは、既定で有効になっています。管理者は、[メッセージング ポリシーを設定](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings)し、**[会話で Giphy を使用する]** が **[オン]** であることを確認することで、ユーザーが Giphy を使用できるかどうかを制御できます。

GIF が Teams 会話で期待どおりに動作しない場合は、次のことを確認します。

[メッセージング ポリシー](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams)で Giphy を許可する必要があります。 PowerShell コマンドレットを使用して確認するには、次の手順に従います。

- [PowerShell を使用して Teams を管理](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)できることを確認します。
- PowerShell コマンド [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) を実行して、**AllowGiphy** が **TRUE** に設定されていることを確認します。
- **AllowGiphy** が **FALSE** に設定されている場合、次の PowerShell コマンド [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps) を実行します。

[オプションの接続エクスペリエンス](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences)を使用するように設定して、Giphy URL にアクセスする必要があります。

> [!NOTE]
> テナントに複数の Teams メッセージング ポリシーが構成されている場合、PowerShell コマンド [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy を使用して影響を受けるユーザーに割り当てられたポリシーの ID を確認することができます。

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
ms.openlocfilehash: 5ee77e57b3bc64d7a04256ab67b691e5205eac56
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/27/2019
ms.locfileid: "39626353"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>ロビーの設定と参加レベルを制御する

ダイヤルイン ユーザー、外部ユーザー、匿名ユーザーを含むすべてのユーザーが Microsoft Teams のロビーをバイパスできるようにするには、PowerShell を使用してこれを行えます。 組織のグローバル会議ポリシーを変更する例を次に示します。

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

現在、このコマンドレットでは Skype for Business PowerShell モジュールを使用する必要があります。 このコマンドレットを使用するための設定方法については、「[PowerShell によるポリシーの管理](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)」を参照してください。

新しいポリシーをセットアップすることができます。そのポリシーはユーザーに適用する必要があります。 グローバル ポリシーを変更した場合、変更されたポリシーは自動的にユーザーに適用されます。 ポリシーを変更した場合、ポリシーが有効になるまで少なくとも 4 時間、最大で 24 時間待つ必要があります。

これらの変更を行う前に、下のドキュメントをよく確認し、許可される内容について正確に理解するようにします。

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Teams の会議ロビー ポリシーの制御の説明

- [[ユーザーの参加を自動的に許可する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)] は開催者単位のポリシーで、ユーザーは会議に直接参加するのか、認証されたユーザーにより入室が許可されるまでロビーで待機するのかを制御します。

- [[匿名ユーザーに会議の開始を許可する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)] は開催者単位のポリシーで、認証された組織のユーザーが参加していない場合でも、B2B ユーザーおよびフェデレーション ユーザーなどの匿名ユーザーがユーザーの会議に参加できるかどうかを制御します。

- [[ダイヤルイン ユーザーによるロビーのバイパスを許可する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)] (**近日公開予定**) は開催者単位のポリシーで、電話を使用してダイヤルインするユーザーは会議に直接参加するのか、[**ユーザーの参加を自動的に許可する**] の設定に関わらずロビーで待機するのかを制御します。

- [[開催者によるロビーの設定の上書きを許可する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)] (**近日公開予定**) は開催者単位のポリシーで、管理者が新しい会議のスケジュール時に設定した [**ユーザーの参加を自動的に許可する**] または [**ダイヤルイン ユーザーによるロビーのバイパスを許可する**] のロビー設定を会議開催者がオーバーライドできるかどうかを制御します。

**注:** Microsoft Teams の会議ポリシーの完全な概要については、「[Teams で会議ポリシーを管理する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)」を参照してください。

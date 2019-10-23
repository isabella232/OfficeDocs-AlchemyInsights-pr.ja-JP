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
# <a name="control-lobby-settings-and-level-of-participation"></a>ロビーの設定と参加レベルの制御

ダイヤルイン、外部、匿名の各ユーザーを含むすべてのユーザーがロビーをバイパスできるようにする場合は、PowerShell を使用して実行できます。 組織のグローバル会議ポリシーを変更する例を次に示します。

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

現在、このコマンドレットでは、Skype for Business PowerShell モジュールを使用する必要があります。 このコマンドレットを使用するには、PowerShell を使用してポリシーを管理することをご確認ください。

新しいポリシーをセットアップして、ユーザーに適用する必要があります。 グローバルポリシーを変更すると、ユーザーに自動的に適用されます。 ポリシーを変更する場合は、ポリシーが有効になるまで、少なくとも4時間、最大24時間待機する必要があります。

このような変更を行う前に、次のドキュメントを必ず確認してください。

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Teams 会議ロビーポリシーコントロールについて

- [[ユーザーに自動的に](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)許可するのは開催者ごとのポリシーで、ユーザーが会議に直接参加するか、認証されたユーザーによって許可されるまでロビーで待機するかを制御します。

- [[匿名ユーザーによる会議の開始を許可](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)する] は、組織の承認されたユーザーが参加していない場合に、B2B ユーザーやフェデレーションユーザーを含む匿名ユーザーがユーザーの会議に参加できるかどうかを制御する、開催者ごとのポリシーです。

- [[ダイヤルインユーザーがロビーをバイパスすることを許可する](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)] (**近日**中に) は、電話でダイヤルインするユーザーが、**自動的にユーザー**の設定に関係なく、ミーティングに直接参加するか、またはロビーで待機するかを制御する開催者ごとのポリシーです。

- [[開催者にロビーの設定を上書きすることを許可](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)する] (**近日**) は開催者ごとのポリシーで、会議の開催者が**自動的にユーザー**を許可し、ダイヤルインを**許可するために管理者が設定したロビー設定を上書きできるかどうかを制御します。ユーザー**が新しい会議をスケジュールするときに、ロビーをバイパスする。

**注:** Microsoft Teams の会議ポリシーの完全な概要については、「 [teams での会議ポリシーの管理](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)」を参照してください。

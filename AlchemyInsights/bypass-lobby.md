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
# <a name="control-lobby-settings-and-level-of-participation"></a>ロビーの設定と参加レベルの制御

これらの設定は、参加者が会議に参加する前にロビーで待機する会議の参加者と、会議で許可されている参加レベルを制御します。 Powershell を使用すると、Teams の管理センターで、まだ実装されていない (「近いうちに」というラベルの) ミーティングポリシー設定を更新できます。  すべてのユーザーがロビーをバイパスできるようにする PowerShell コマンドレットの例については、以下を参照してください。  

- [[ユーザーに自動的に](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)許可するのは開催者ごとのポリシーで、ユーザーが会議に直接参加するか、認証されたユーザーによって許可されるまでロビーで待機するかを制御します。

- [[匿名ユーザーによる会議の開始を許可](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)する] は、組織の承認されたユーザーが参加していない場合に、B2B ユーザーやフェデレーションユーザーを含む匿名ユーザーがユーザーの会議に参加できるかどうかを制御する、開催者ごとのポリシーです。

- [[ダイヤルインユーザーがロビーをバイパスすることを許可する](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)] (**近日**中に) は、電話でダイヤルインするユーザーが、**自動的にユーザー**の設定に関係なく、ミーティングに直接参加するか、またはロビーで待機するかを制御する開催者ごとのポリシーです。

- [[開催者にロビーの設定を上書きすることを許可](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)する] (**近日**) は開催者ごとのポリシーで、会議の開催者が**自動的にユーザー**を許可し、ダイヤルインを**許可するために管理者が設定したロビー設定を上書きできるかどうかを制御します。ユーザー**が新しい会議をスケジュールするときに、ロビーをバイパスする。

**注:** Microsoft Teams の会議ポリシーの完全な概要については、「 [teams での会議ポリシーの管理](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)」を参照してください。 


**PowerShell の例**

外部または匿名ユーザーを含むすべてのユーザーがロビーをバイパスできるようにする場合は、PowerShell を使用してこのタスクを実行することもできます。  ここでは、組織のグローバル会議ポリシーを変更する例を示します。   

(この変更を行う前に、上記のドキュメントを必ずご確認ください)。

CsTeamsMeetingPolicy-Identity Global-AutoAdmittedUsers 「Everyone」-AllowPSTNUsersToBypassLobby $True

詳細については、「 [CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps)」を参照してください。

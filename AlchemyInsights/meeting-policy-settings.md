---
title: 会議ポリシーの設定
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/02/2019
ms.locfileid: "37380100"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Microsoft Teams での会議ポリシーの管理

会議ポリシーは、組織内のユーザーによってスケジュールされた会議の会議参加者が使用できる機能を制御するために使用されます。 会議ポリシーの一部の機能は、Teams 管理センターには実装されていない場合があります (ドキュメントの「近日中」というラベルが付いています)。 この場合、または Microsoft Teams の管理センターで "ポリシーを今すぐには更新できません。後でもう一度実行してください" のようなエラーが表示される場合は、PowerShell を使用して Teams の会議ポリシーを作成または変更することをお勧めします。 

会議ポリシーの詳細については、次のリソースを参照してください。

- ポリシーの作成、変更、およびポリシーへのユーザーの割り当てについては、「 [Teams での会議ポリシーの管理](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)」を参照してください。

- PowerShell コマンドレットを使用してポリシーを変更するには、「 [Teams powershell の概要](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)」を参照してください。 
    - Teams の会議ポリシーには、 [Skype For Business PowerShell モジュール](https://www.microsoft.com/download/details.aspx?id=39366)を使用する必要があります。 
    - 詳細については、 [CsTeamsMeetingPolicy コマンドレットのドキュメント](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)を参照してください。

**注:** ユーザーがポリシーの変更を有効にするには、最大24時間かかる場合があります。 新しく作成したポリシーをすぐに変更できない場合があります。4時間待ってから、新しく作成したポリシーをもう一度変更します。 それでも問題が解決しない場合は、PowerShell をお試しください。  
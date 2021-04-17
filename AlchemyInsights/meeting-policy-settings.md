---
title: 会議ポリシーの設定
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825448"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Microsoft Teams で会議ポリシーを管理する

**注: ポリシーの変更がユーザーに反映されるまで最大 24 時間かかる場合があります。** 新しく作成されたポリシーをすぐに変更できない場合があります。4 時間待ってから、新しく作成されたポリシーを再度変更してみてください。

会議ポリシーは、組織内のユーザーによってスケジュールされた会議への参加者が利用できる機能を制御するために使用されます。 会議ポリシーの一部の機能は、Teams 管理センターにまだ実装されていない場合があります (これらはドキュメントに "近日公開" としてラベル付けされています)。 この場合、もしくは Microsoft Teams 管理センターで "今すぐポリシーを更新することはできませんが、後でもう一度試してください" などのエラーが表示される場合には、PowerShell を使用して Teams 会議ポリシーを作成または変更することをお勧めします。 

会議ポリシーの詳細については、以下のリソースをご覧ください。

- ポリシーの作成、変更、およびポリシーへのユーザーの割り当ての詳細については、「[Teams での会議ポリシーを管理する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)」を参照してください。

- PowerShell コマンドレットを使用してポリシーを変更するには、「[Teams での PowerShell の概要](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)」を参照してください。 
    - Teams の会議ポリシーには、[Skype for Business PowerShell モジュール](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector)を使用する必要があります。 
    - 詳細については、[*-CsTeamsMeetingPolicy コマンドレットのドキュメント](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)を参照してください。


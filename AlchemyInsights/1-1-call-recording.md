---
title: 1 対 1 通話のレコーディング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314389"
---
# <a name="11-call-recording"></a>1 対 1 通話のレコーディング

1 対 1 通話で **[録音の開始]** ボタンがグレー表示されている場合は、影響を受けるユーザーのポリシー設定を変更する必要があります。 ポリシー設定を確認するには、上記の「**Diag: Teams 1 対 1 通話のレコーディング**」と入力して、影響を受けるユーザーの診断を実行します。     

2021 年 5 月 31 日から、新しい Teams 通話ポリシー  *AllowCloudRecordingForCalls* の適用を開始します。 この変更の前は、1 対 1 通話のレコーディングは *AllowCloudRecording* Teams 会議ポリシーによって制御されていました。 この変更は、メッセージ センターの投稿に記載されています:  [(更新) 1 対 1 通話レコーディング ポリシーの紹介](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)。  

*AllowCloudRecordingForCalls*  通話ポリシー オプションは、既定で **$False** に設定されています。 すべてのユーザーに 1 対 1 通話のレコーディングを禁止する場合は、何もする必要はありません。  

1 対 1 通話ですべてのユーザーの通話のレコーディングを有効にするには、 [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) を使用して次のコマンドレットを実行します。 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

または、新しいポリシーを作成して **-AllowCloudRecordingForCalls** を **$true** に設定し、そのポリシーをユーザーに割り当てることもできます。 

詳細については、「[1 対 1 通話レコーディング ポリシー制御は (ほぼ) ここにあります](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)」を参照してください。

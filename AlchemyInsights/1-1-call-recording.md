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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733854"
---
# <a name="11-call-recording"></a>1 対 1 通話のレコーディング

管理者は、ユーザーが 1 対 1 通話を録音できるようにするため、今すぐアクションを実行する必要があります。
 
2021 年 4 月 12 日から、新しい Teams 通話ポリシー オプション *AllowCloudRecordingForCalls* の適用を開始します。 

現在、1 対 1 通話のレコーディング機能は、Teams 会議ポリシーの *AllowCloudRecording* オプションによって制御されています。 ユーザーが Teams 会議の録音を許可されている場合は、1 対 1 通話を録音することもできます。

すべてのユーザーに 1 対 1 通話の録音を禁止する場合は、何もする必要はありません。 *AllowCloudRecordingForCalls* 通話ポリシー オプションは、既定で $False になります。

この変更は、次のメッセージ センターの投稿に記載されています: [(更新) 1 対 1 通話のレコーディング ポリシーの概要](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Teams 通話ポリシー オプションを設定するには、[Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) を使用する必要があります。

**1 対 1 通話で通話レコーディングを有効にするには:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**1 対 1 通話で通話レコーディングを無効にするには:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False


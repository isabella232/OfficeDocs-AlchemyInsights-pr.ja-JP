---
title: ホステッド ボイスメールを有効にする方法
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055559"
---
# <a name="how-to-enable-hosted-voicemail"></a>ホステッド ボイスメールを有効にする方法

ボイスメールを有効にするには、**HostedVoicemail** を $true に設定する必要があります。

リモート PowerShell (RPS) を使用するユーザーの **HostedVoicemail** プロパティです。

RPS への接続の詳細については、「[Microsoft Teams PowerShell の概要](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)」を参照してください。

1. Teams 管理者は、Teams のリモート PowerShell にログインする必要があります。
1. PowerShell プロンプトから、Teams 管理者は **set-csuser user@contoso.com -HostedVoiceMail $true** を実行できます。ここで、sip uri は問題のユーザーです。

> [!NOTE]
> ポリシーの変更を複製するには、最大 24 時間かかります。
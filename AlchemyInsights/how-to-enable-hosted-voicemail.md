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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318653"
---
# <a name="how-to-enable-hosted-voicemail"></a>ホステッド ボイスメールを有効にする方法

ボイスメールを有効にするには、**HostedVoicemail** を $true に設定する必要があります。

リモート PowerShell (RPS) を使用するユーザーの **HostedVoicemail** プロパティです。

RPS への接続の詳細については、「[Microsoft Teams PowerShell の概要](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)」を参照してください。

1. Teams 管理者は、Teams のリモート PowerShell にログインする必要があります。
1. PowerShell プロンプトから、Teams 管理者は **set-csuser user@contoso.com -HostedVoiceMail $true** を実行できます。ここで、sip uri は問題のユーザーです。

**注**: ポリシーの変更を複製するには、最大 24 時間かかります。
---
title: デバイスを有効にする
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
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2021
ms.locfileid: "50257025"
---
# <a name="enable-device"></a>デバイスを有効にする

**Powershell コマンドを使ってデバイスを有効にするには**

以下のコマンドを実行します。

- デバイス オブジェクトを取得する: `Get-MsolDevice -Name <Name>`
- デバイスを有効にする: `Enable-MsolDevice -DeviceId <DeviceId>`

管理対象ドメインでの Hybrid Join の構成に関する詳細については、「[Hybrid Join を構成する](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)」を参照してください。

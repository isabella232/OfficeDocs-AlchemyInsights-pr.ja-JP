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
ms.openlocfilehash: 4722ccf6847fc6c02616dbc62d59a2a87c089f77ae79c0a916211af6c5f2a6d0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003491"
---
# <a name="enable-device"></a>デバイスを有効にする

**Powershell コマンドを使ってデバイスを有効にするには**

以下のコマンドを実行します。

- デバイス オブジェクトを取得する: `Get-MsolDevice -Name <Name>`
- デバイスを有効にする: `Enable-MsolDevice -DeviceId <DeviceId>`

管理対象ドメインでの Hybrid Join の構成に関する詳細については、「[Hybrid Join を構成する](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)」を参照してください。

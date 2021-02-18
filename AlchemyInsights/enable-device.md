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
# <a name="enable-device"></a><span data-ttu-id="d1c90-102">デバイスを有効にする</span><span class="sxs-lookup"><span data-stu-id="d1c90-102">Enable Device</span></span>

<span data-ttu-id="d1c90-103">**Powershell コマンドを使ってデバイスを有効にするには**</span><span class="sxs-lookup"><span data-stu-id="d1c90-103">**To enable the device using Powershell command**</span></span>

<span data-ttu-id="d1c90-104">以下のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="d1c90-104">Run the following commands:</span></span>

- <span data-ttu-id="d1c90-105">デバイス オブジェクトを取得する: `Get-MsolDevice -Name <Name>`</span><span class="sxs-lookup"><span data-stu-id="d1c90-105">To get device object: `Get-MsolDevice -Name <Name>`</span></span>
- <span data-ttu-id="d1c90-106">デバイスを有効にする: `Enable-MsolDevice -DeviceId <DeviceId>`</span><span class="sxs-lookup"><span data-stu-id="d1c90-106">To enable device: `Enable-MsolDevice -DeviceId <DeviceId>`</span></span>

<span data-ttu-id="d1c90-107">管理対象ドメインでの Hybrid Join の構成に関する詳細については、「[Hybrid Join を構成する](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1c90-107">For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span></span>

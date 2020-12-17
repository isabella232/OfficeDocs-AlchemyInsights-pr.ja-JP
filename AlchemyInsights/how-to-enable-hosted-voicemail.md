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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/09/2020
ms.locfileid: "49680480"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="c87b4-102">ホステッド ボイスメールを有効にする方法</span><span class="sxs-lookup"><span data-stu-id="c87b4-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="c87b4-103">ボイスメールを有効にするには、**HostedVoicemail** を $true に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c87b4-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="c87b4-104">リモート PowerShell (RPS) を使用するユーザーの **HostedVoicemail** プロパティです。</span><span class="sxs-lookup"><span data-stu-id="c87b4-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="c87b4-105">RPS への接続の詳細については、「[Microsoft Teams PowerShell の概要](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c87b4-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="c87b4-106">Teams 管理者は、Teams のリモート PowerShell にログインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c87b4-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="c87b4-107">PowerShell プロンプトから、Teams 管理者は **set-csuser user@contoso.com -HostedVoiceMail $true** を実行できます。ここで、sip uri は問題のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="c87b4-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="c87b4-108">ポリシーの変更を複製するには、最大 24 時間かかります。</span><span class="sxs-lookup"><span data-stu-id="c87b4-108">Changes to policies can take up to 24 hours to replicate.</span></span>
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
# <a name="11-call-recording"></a><span data-ttu-id="a853d-102">1 対 1 通話のレコーディング</span><span class="sxs-lookup"><span data-stu-id="a853d-102">1:1 call recording</span></span>

<span data-ttu-id="a853d-103">管理者は、ユーザーが 1 対 1 通話を録音できるようにするため、今すぐアクションを実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a853d-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="a853d-104">2021 年 4 月 12 日から、新しい Teams 通話ポリシー オプション *AllowCloudRecordingForCalls* の適用を開始します。</span><span class="sxs-lookup"><span data-stu-id="a853d-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="a853d-105">現在、1 対 1 通話のレコーディング機能は、Teams 会議ポリシーの *AllowCloudRecording* オプションによって制御されています。</span><span class="sxs-lookup"><span data-stu-id="a853d-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="a853d-106">ユーザーが Teams 会議の録音を許可されている場合は、1 対 1 通話を録音することもできます。</span><span class="sxs-lookup"><span data-stu-id="a853d-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="a853d-107">すべてのユーザーに 1 対 1 通話の録音を禁止する場合は、何もする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="a853d-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="a853d-108">*AllowCloudRecordingForCalls* 通話ポリシー オプションは、既定で $False になります。</span><span class="sxs-lookup"><span data-stu-id="a853d-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="a853d-109">この変更は、次のメッセージ センターの投稿に記載されています: [(更新) 1 対 1 通話のレコーディング ポリシーの概要](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Teams 通話ポリシー オプションを設定するには、[Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a853d-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="a853d-110">**1 対 1 通話で通話レコーディングを有効にするには:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="a853d-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="a853d-111">**1 対 1 通話で通話レコーディングを無効にするには:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="a853d-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>


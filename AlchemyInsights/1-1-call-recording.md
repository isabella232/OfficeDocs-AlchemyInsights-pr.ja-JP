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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696963"
---
# <a name="11-call-recording"></a><span data-ttu-id="176b8-102">1 対 1 通話のレコーディング</span><span class="sxs-lookup"><span data-stu-id="176b8-102">1:1 call recording</span></span>

<span data-ttu-id="176b8-103">1 対 1 通話で **[録音の開始]** ボタンがグレー表示されている場合は、影響を受けるユーザーのポリシー設定を変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="176b8-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="176b8-104">2021 年 5 月 31 日から、新しい Teams 通話ポリシー  *AllowCloudRecordingForCalls* の適用を開始します。</span><span class="sxs-lookup"><span data-stu-id="176b8-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="176b8-105">この変更の前は、1 対 1 通話のレコーディングは *AllowCloudRecording* Teams 会議ポリシーによって制御されていました。</span><span class="sxs-lookup"><span data-stu-id="176b8-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="176b8-106">この変更は、メッセージ センターの投稿に記載されています:  [(更新) 1 対 1 通話レコーディング ポリシーの紹介](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)。</span><span class="sxs-lookup"><span data-stu-id="176b8-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="176b8-107">*AllowCloudRecordingForCalls*  通話ポリシー オプションは、既定で **$False** に設定されています。</span><span class="sxs-lookup"><span data-stu-id="176b8-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="176b8-108">すべてのユーザーに 1 対 1 通話のレコーディングを禁止する場合は、何もする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="176b8-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="176b8-109">1 対 1 通話ですべてのユーザーの通話のレコーディングを有効にするには、Teams PowerShell を使用して次のコマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="176b8-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="176b8-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="176b8-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="176b8-111">または、新しいポリシーを作成して **-AllowCloudRecordingForCalls** を **$true** に設定し、そのポリシーをユーザーに割り当てることもできます。</span><span class="sxs-lookup"><span data-stu-id="176b8-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="176b8-112">詳細については、「[1 対 1 通話レコーディング ポリシー制御は (ほぼ) ここにあります](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="176b8-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>

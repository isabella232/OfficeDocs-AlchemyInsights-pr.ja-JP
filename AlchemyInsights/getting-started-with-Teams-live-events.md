---
title: Teams のライブ イベントの使用を開始する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811965"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="365af-102">Teams のライブ イベントの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="365af-102">Getting started with Teams live events</span></span>

<span data-ttu-id="365af-103">Microsoft Teams のライブ イベントは Teams 会議の拡張機能であり、これを使用すると、多くのオンライン視聴者にストリーミングするイベントのスケジュールと作成を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="365af-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="365af-104">ライブ イベントの作成には、以下のものが必要です。</span><span class="sxs-lookup"><span data-stu-id="365af-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="365af-105">まず、Teams のライブ イベントが[お客様の国と地域で利用可能](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability)であることをご確認ください。ライブ イベントは、一部の国ではまだサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="365af-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="365af-106">ライセンスを割り当ててポリシーを設定したにもかかわらず Teams のライブ イベントを作成できない場合、お住まいの国または地域でライブ イベントがまだ提供されていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="365af-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="365af-107">[Office 365 Enterprise E1、E3、E5 のいずれかのライセンス、または Office 365 A3 または A5 ライセンス](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses)。</span><span class="sxs-lookup"><span data-stu-id="365af-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="365af-108">**注**: Teams の使用数が最近増加したため、Teams ライセンスをユーザーに割り当てると、完全にセットアップされるまでに約 24 時間かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="365af-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="365af-109">それまでの間、Teams ポリシーの割り当てを行うことはできません。また、通話や電話会議など一部の Teams 機能を利用できないことがあります。</span><span class="sxs-lookup"><span data-stu-id="365af-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="365af-110">[Microsoft Teams 管理センターでのライブ イベントを作成する](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy)ためのアクセス許可。</span><span class="sxs-lookup"><span data-stu-id="365af-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="365af-111">[Microsoft Stream でのライブ イベントを作成する](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events)ためのアクセス許可 (外部へのブロードキャストのアプリまたはデバイスを使用して作成されたイベントの場合)。</span><span class="sxs-lookup"><span data-stu-id="365af-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="365af-112">組織内の完全なチーム メンバーシップ (ゲストや別の組織のメンバーは不可)。</span><span class="sxs-lookup"><span data-stu-id="365af-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="365af-113">プライベート会議のスケジュール、画面共有、IP ビデオの共有は、Teams の会議ポリシーでは有効になります。</span><span class="sxs-lookup"><span data-stu-id="365af-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="365af-114">Teams のライブ イベントの[ベスト プラクティス](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42)。</span><span class="sxs-lookup"><span data-stu-id="365af-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="365af-115">詳細については、「[Microsoft Teams ライブ イベントの使用を開始する](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="365af-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>
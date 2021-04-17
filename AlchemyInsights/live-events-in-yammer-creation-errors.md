---
title: Yammer 作成エラーのライブ イベント
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
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825520"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="58be3-102">Yammer 作成エラーのライブ イベント</span><span class="sxs-lookup"><span data-stu-id="58be3-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="58be3-103">**Yammer ライブ イベントの作成**</span><span class="sxs-lookup"><span data-stu-id="58be3-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="58be3-104">Yammer には、常にライブ イベントの作成をするオプションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="58be3-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="58be3-105">場合によっては、ユーザーがライブ イベント作成の前提条件を満たしていないことがあり、ユーザーが作成しようとしたときにエラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="58be3-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="58be3-106">以下では、この問題の一般的な理由について説明し、エンドユーザーが問題を解決する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="58be3-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="58be3-107">**ライブ イベントを作成できるユーザー**</span><span class="sxs-lookup"><span data-stu-id="58be3-107">**Who can create live events**</span></span>
- <span data-ttu-id="58be3-108">Office 365 Enterprise E1、E3、E5 のいずれかのライセンス、または Office 365 A3 または A5 ライセンスがある。</span><span class="sxs-lookup"><span data-stu-id="58be3-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="58be3-109">Microsoft Teams 管理センターでのライブ イベントを作成するためのアクセスを許可されている。</span><span class="sxs-lookup"><span data-stu-id="58be3-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="58be3-110">Microsoft Stream でのライブ イベントを作成するためのアクセスを許可されている (外部へのブロードキャストのアプリまたはデバイスを使用して作成されたイベントの場合)。</span><span class="sxs-lookup"><span data-stu-id="58be3-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="58be3-111">組織内の完全なチーム メンバーシップがある (ゲストや別の組織のメンバーは不可)。</span><span class="sxs-lookup"><span data-stu-id="58be3-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="58be3-112">プライベート会議のスケジュール、画面共有、IP ビデオの共有は、Teams の会議ポリシーでは有効になります。</span><span class="sxs-lookup"><span data-stu-id="58be3-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="58be3-113">**ライブ イベントの作成のポリシー**</span><span class="sxs-lookup"><span data-stu-id="58be3-113">**Live event creation policies**</span></span>

<span data-ttu-id="58be3-114">Yammer は、ストリーム用の Office 365 テナントに設定されているライブ イベントポリシーに従います。</span><span class="sxs-lookup"><span data-stu-id="58be3-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="58be3-115">既定では、組織内のすべてのユーザーがライブ イベントを作成できます。</span><span class="sxs-lookup"><span data-stu-id="58be3-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="58be3-116">管理者が[この設定を変更すると、ユーザーがライブ イベントを作成できなくなる可能性があり ます](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)。</span><span class="sxs-lookup"><span data-stu-id="58be3-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="58be3-117">ユーザーがポリシーエラーを受信した場合、ライブ イベントを作成する権限があることを確認することが重要です。</span><span class="sxs-lookup"><span data-stu-id="58be3-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>

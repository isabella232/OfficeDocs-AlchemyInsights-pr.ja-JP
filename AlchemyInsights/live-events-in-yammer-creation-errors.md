---
title: Yammer 作成エラーのライブ イベント
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 35cddfee1a78fd6e1e502871bd5b56d786bf300a
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/30/2020
ms.locfileid: "44012646"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="ebaf6-102">Yammer 作成エラーのライブ イベント</span><span class="sxs-lookup"><span data-stu-id="ebaf6-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="ebaf6-103">**Yammer ライブ イベントの作成**</span><span class="sxs-lookup"><span data-stu-id="ebaf6-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="ebaf6-104">Yammer には、常にライブ イベントの作成をするオプションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ebaf6-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="ebaf6-105">場合によっては、ユーザーがライブ イベント作成の前提条件を満たしていないことがあり、ユーザーが作成しようとしたときにエラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ebaf6-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="ebaf6-106">以下では、この問題の一般的な理由について説明し、エンドユーザーが問題を解決する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="ebaf6-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="ebaf6-107">**ライブ イベントを作成できるユーザー**</span><span class="sxs-lookup"><span data-stu-id="ebaf6-107">**Who can create live events**</span></span>
- <span data-ttu-id="ebaf6-108">Office 365 Enterprise E1、E3、E5 のいずれかのライセンス、または Office 365 A3 または A5 ライセンスがある。</span><span class="sxs-lookup"><span data-stu-id="ebaf6-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="ebaf6-109">Microsoft Teams 管理センターでのライブ イベントを作成するためのアクセスを許可されている。</span><span class="sxs-lookup"><span data-stu-id="ebaf6-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="ebaf6-110">Microsoft Stream でのライブ イベントを作成するためのアクセスを許可されている (外部へのブロードキャストのアプリまたはデバイスを使用して作成されたイベントの場合)。</span><span class="sxs-lookup"><span data-stu-id="ebaf6-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="ebaf6-111">組織内の完全なチーム メンバーシップがある (ゲストや別の組織のメンバーは不可)。</span><span class="sxs-lookup"><span data-stu-id="ebaf6-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="ebaf6-112">プライベート会議のスケジュール、画面共有、IP ビデオの共有は、Teams の会議ポリシーでは有効になります。</span><span class="sxs-lookup"><span data-stu-id="ebaf6-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="ebaf6-113">**ライブ イベントの作成のポリシー**</span><span class="sxs-lookup"><span data-stu-id="ebaf6-113">**Live event creation policies**</span></span>

<span data-ttu-id="ebaf6-114">Yammer は、ストリーム用の Office 365 テナントに設定されているライブ イベントポリシーに従います。</span><span class="sxs-lookup"><span data-stu-id="ebaf6-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="ebaf6-115">既定では、組織内のすべてのユーザーがライブ イベントを作成できます。</span><span class="sxs-lookup"><span data-stu-id="ebaf6-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="ebaf6-116">管理者が[この設定を変更すると、ユーザーがライブ イベントを作成できなくなる可能性があり ます](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)。</span><span class="sxs-lookup"><span data-stu-id="ebaf6-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="ebaf6-117">ユーザーがポリシーエラーを受信した場合、ライブ イベントを作成する権限があることを確認することが重要です。</span><span class="sxs-lookup"><span data-stu-id="ebaf6-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>

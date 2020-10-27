---
title: 教育機関で会議記録を管理する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6131"
- "9002530"
ms.openlocfilehash: 144480dbed8b74f8b395b6b80c586038a1f12697
ms.sourcegitcommit: e1d72cf118451ed62e975970e5a2faa4b13282f5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/24/2020
ms.locfileid: "48753676"
---
# <a name="manage-meeting-recordings-for-education"></a><span data-ttu-id="cc4f7-102">教育機関で会議記録を管理する</span><span class="sxs-lookup"><span data-stu-id="cc4f7-102">Manage meeting recordings for Education</span></span>

<span data-ttu-id="cc4f7-103">**2020 年 8 月 20 日** 以降、A1 (A1 Plus を含む) ライセンスを持つユーザーが Teams 会議の記録を開始すると、記録は 21 日間利用できます。</span><span class="sxs-lookup"><span data-stu-id="cc4f7-103">Starting **August 20, 2020** , when users with A1 (including A1 Plus) licenses start a Teams meeting recording, the recording is available for 21 days.</span></span>

<span data-ttu-id="cc4f7-104">会議を別の場所に保存する方法など、詳細については、「[Microsoft Teams 会議の記録を Stream にアップロードする](https://docs.microsoft.com/stream/portal-upload-teams-meeting-recording)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="cc4f7-104">For more info, including how to save the meeting to another location, see [Upload a Microsoft Teams meeting recording to Stream](https://docs.microsoft.com/stream/portal-upload-teams-meeting-recording).</span></span>

<span data-ttu-id="cc4f7-105">Microsoft Teams 会議の記録を OneDrive SharePoint に保存できるようになりました。詳細とオプトインについては、次のメッセージ センターの投稿を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc4f7-105">Microsoft Teams Meeting Recording can now be stored in OneDrive SharePoint, for more information and to opt-in, see the following Message Center Post:</span></span>

[<span data-ttu-id="cc4f7-106">(更新) Microsoft Teams: OneDrive と SharePoint に保存された会議の記録</span><span class="sxs-lookup"><span data-stu-id="cc4f7-106">(Updated) Microsoft Teams: meeting recordings saved to OneDrive and SharePoint</span></span>](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter&id=MC222640)

<span data-ttu-id="cc4f7-107">ストレージの場所を OneDrive と SharePoint に移動すると、お住まいの地域で Stream を使用できるという以前の要件がなくなります。</span><span class="sxs-lookup"><span data-stu-id="cc4f7-107">Moving your storage location to OneDrive and SharePoint eliminates the previous requirement that Stream be available in your region.</span></span>

<span data-ttu-id="cc4f7-108">学生が Teams で会議を記録するのを **ブロックまたは有効にする** 方法を探している場合は、学生と教育者の安全のためにポリシー パッケージを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="cc4f7-108">If you’re looking for how to **block or enable** students to Record Meetings in Teams, we recommend using policy packages for student and educator safety.</span></span> <span data-ttu-id="cc4f7-109">詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc4f7-109">For more info, see:</span></span>

<span data-ttu-id="cc4f7-110">[Microsoft Teams のポリシー パッケージ](https://docs.microsoft.com/microsoftteams/policy-packages-edu#policy-packages-in-microsoft-teams)。</span><span class="sxs-lookup"><span data-stu-id="cc4f7-110">[Policy packages in Microsoft Teams](https://docs.microsoft.com/microsoftteams/policy-packages-edu#policy-packages-in-microsoft-teams).</span></span>

<span data-ttu-id="cc4f7-111">[学生の安全を保証するために割り当てるべきポリシー](https://docs.microsoft.com/microsoftteams/policy-packages-edu#policies-that-should-be-assigned-for-student-safety)。</span><span class="sxs-lookup"><span data-stu-id="cc4f7-111">[Policies that should be assigned for student safety](https://docs.microsoft.com/microsoftteams/policy-packages-edu#policies-that-should-be-assigned-for-student-safety).</span></span>

<span data-ttu-id="cc4f7-112">[教師向けに割り当てるべきポリシー](https://docs.microsoft.com/microsoftteams/policy-packages-edu#policies-that-should-be-assigned-for-educators)。</span><span class="sxs-lookup"><span data-stu-id="cc4f7-112">[Policies that should be assigned for educators](https://docs.microsoft.com/microsoftteams/policy-packages-edu#policies-that-should-be-assigned-for-educators).</span></span>

<span data-ttu-id="cc4f7-113">会議を記録する機能のみを管理する場合は、「[クラウド レコーディングを開始または停止する](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)」の を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc4f7-113">If you want to manage only the ability to record meetings, see [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>

<span data-ttu-id="cc4f7-114">**注** Teams 会議の記録で OneDrive SharePoint ストレージをオプトインしていない限り、これらの機能は Stream の地域および国の可用性に依存します。</span><span class="sxs-lookup"><span data-stu-id="cc4f7-114">**Note** Unless you have opted in to OneDrive SharePoint storage for Teams Meeting Recordings, those capabilities rely on Stream regional and country availability.</span></span> <span data-ttu-id="cc4f7-115">会議を記録できない場合は、「[Microsoft Stream は、どの地域にデータをホストしますか](https://docs.microsoft.com/stream/faq#which-regions-does-microsoft-stream-host-my-data-in)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc4f7-115">If you can't record a meeting, see [Which regions does Microsoft Stream host my data in?](https://docs.microsoft.com/stream/faq#which-regions-does-microsoft-stream-host-my-data-in).</span></span>

<span data-ttu-id="cc4f7-116">詳細については、「[更新された機能: Microsoft Stream クラウド レコーディング地域ストレージ制御](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter?id=MC214327)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc4f7-116">For more information, see [Updated Feature: Microsoft Stream cloud recordings regional storage control](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter?id=MC214327).</span></span>
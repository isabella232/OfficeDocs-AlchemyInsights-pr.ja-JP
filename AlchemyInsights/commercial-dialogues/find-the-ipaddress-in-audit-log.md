---
title: 監査ログで IP アドレスを見つける
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484150"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="cae3f-102">監査ログで IP アドレスを見つける</span><span class="sxs-lookup"><span data-stu-id="cae3f-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="cae3f-103">ユーザーまたは管理者によって実行されたアクティビティに対応する IP アドレスが監査ログに表示されます。</span><span class="sxs-lookup"><span data-stu-id="cae3f-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="cae3f-104">クライアント情報も記録されます。</span><span class="sxs-lookup"><span data-stu-id="cae3f-104">The client information is also logged.</span></span> <span data-ttu-id="cae3f-105">IP アドレスを特定する方法は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="cae3f-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="cae3f-106">[Office 365 セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/p/?linkid=2077143)に移動します。</span><span class="sxs-lookup"><span data-stu-id="cae3f-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="cae3f-107">**[検索]** > **[ [監査ログ検索]](https://go.microsoft.com/fwlink/?linkid=2103759)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="cae3f-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="cae3f-108">監査を有効にする必要があるという通知が表示された場合は、先に進んで今すぐ有効にしてください。</span><span class="sxs-lookup"><span data-stu-id="cae3f-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="cae3f-109">この機能が有効になっていない場合、検索結果は前の日付からデータを取得できません。</span><span class="sxs-lookup"><span data-stu-id="cae3f-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="cae3f-110">特定のアクティビティに興味がある場合は、**[アクティビティ]** リストから選択してください。 それ以外の場合、既定では、選択したユーザーのすべてのアクティビティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cae3f-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="cae3f-111">特定のアクティビティは、**[アクティビティ]** メニューから選択できない場合があることに注意してください。 ただし、**[すべてのアクティビティの結果を表示する]** が選択されている場合 (既定設定)、これらの監査項目が返されます。</span><span class="sxs-lookup"><span data-stu-id="cae3f-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="cae3f-112">日付範囲を指定し、**[ユーザー]** フィールドで、調査するユーザーのユーザー名を選択します。</span><span class="sxs-lookup"><span data-stu-id="cae3f-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="cae3f-113">**[検索]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="cae3f-113">Select **Search**.</span></span> <span data-ttu-id="cae3f-114">アクティビティは **[結果]** の下に表示されます。</span><span class="sxs-lookup"><span data-stu-id="cae3f-114">The activities appear under **Results**.</span></span> <span data-ttu-id="cae3f-115">各アクティビティの IP アドレスを確認できます。</span><span class="sxs-lookup"><span data-stu-id="cae3f-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="cae3f-116">詳細を表示するには、アクティビティを選択してから、**[詳細情報]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="cae3f-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="cae3f-117">詳細については、「[Office 365 監査ログを検索して一般的なシナリオのトラブルシューティングを行う](https://go.microsoft.com/fwlink/?linkid=2103944)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cae3f-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
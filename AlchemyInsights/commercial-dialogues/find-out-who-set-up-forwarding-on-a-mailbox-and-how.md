---
title: メールボックスに転送を設定したユーザーとその方法を確認する
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484113"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="3ed19-102">メールボックスに転送を設定したユーザーとその方法を確認する</span><span class="sxs-lookup"><span data-stu-id="3ed19-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="3ed19-103">メールボックスに外部転送が設定されている場合、アクティビティは Set-Mailbox コマンドレットの一部として監査されます。</span><span class="sxs-lookup"><span data-stu-id="3ed19-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="3ed19-104">監査ログでアクティビティを見つける方法は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="3ed19-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="3ed19-105">[Office 365 セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/p/?linkid=2077143)に移動します。</span><span class="sxs-lookup"><span data-stu-id="3ed19-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="3ed19-106">**[検索]**> **[監査ログ検索]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3ed19-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="3ed19-107">監査を有効にする必要があるという通知が表示された場合は、先に進んで今すぐ有効にしてください。</span><span class="sxs-lookup"><span data-stu-id="3ed19-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="3ed19-108">この機能が有効になっていない場合、検索結果は前の日付からデータを取得できません。</span><span class="sxs-lookup"><span data-stu-id="3ed19-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="3ed19-109">[**アクティビティ**] フィールドが [**すべてのアクティビティの結果を表示**] (既定) と設定されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="3ed19-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="3ed19-110">日付範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ed19-110">Specify the date range.</span></span> <span data-ttu-id="3ed19-111">ユーザー名を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="3ed19-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="3ed19-112">**[検索]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3ed19-112">Select **Search**.</span></span> <span data-ttu-id="3ed19-113">アクティビティは **[結果]** の下に表示されます。</span><span class="sxs-lookup"><span data-stu-id="3ed19-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="3ed19-114">**[結果をフィルター]** を選択し、[**アクティビティ** フィルター] フィールドに **Set-mailbox** と入力します。</span><span class="sxs-lookup"><span data-stu-id="3ed19-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="3ed19-115">これにより、すべての **Set-Mailbox** アクティビティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3ed19-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="3ed19-116">詳細を表示するには、アクティビティを選択してから、**[詳細情報]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3ed19-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="3ed19-117">**[パラメータ]** の下に、メール ボックスに設定された転送メール アドレスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="3ed19-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="3ed19-118">**[UserID]** は、メール ボックスに外部転送を設定したユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="3ed19-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="3ed19-119">詳細については、「[Office 365 監査ログを検索して一般的なシナリオのトラブルシューティングを行う](https://go.microsoft.com/fwlink/?linkid=2103944)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3ed19-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
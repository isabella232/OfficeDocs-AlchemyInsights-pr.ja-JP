---
title: 削除されたイベントの監査ログを読み取る
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484109"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="fc5fc-102">削除されたイベントの監査ログを読み取る</span><span class="sxs-lookup"><span data-stu-id="fc5fc-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="fc5fc-103">手順は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-103">Here's how to do this:</span></span>

1. <span data-ttu-id="fc5fc-104">[Office 365 セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/p/?linkid=2077143)に移動します。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="fc5fc-105">**[検索]** > [**[監査ログ検索]**](https://go.microsoft.com/fwlink/?linkid=2103759) を選択します。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="fc5fc-106">この機能を有効にする必要があるという通知が表示された場合は、先に進んで今すぐ有効にしてください。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="fc5fc-107">この機能が有効になっていない場合、検索結果は前の日付からデータを取得できません。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="fc5fc-108">**[アクティビティ]** を選択し、**[Exchange メール ボックス アクティビティ]** を検索します。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="fc5fc-109">**[削除済みアイテムフォルダからの削除済みメッセージ]** および **[削除済みアイテム フォルダに移動済みのメッセージ]** オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="fc5fc-110">完了したら、ウィンドウの外側をクリックして、**[アクティビティ]** ウィンドウを最小化します。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="fc5fc-111">日付範囲を指定し、**[ユーザー]** ボックス、調査するユーザーのユーザー名を選択します。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="fc5fc-112">一度に複数のエントリを選択できます。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="fc5fc-113">**[検索]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-113">Select **Search**.</span></span> <span data-ttu-id="fc5fc-114">アクティビティは **[結果]** の下に表示されます。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="fc5fc-115">詳細を表示するには、アクティビティを選択してから、**[詳細情報]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="fc5fc-116">削除された項目に関する追加情報(件名、項目が削除されたときの場所など) は、 [**対象アイテム**] フィールドに表示されます。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="fc5fc-117">監査ログ機能を使用して、削除したアイテムを復元することはできません。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="fc5fc-118">削除済みアイテムを復元する方法については、「[Outlook Web App で削除済みのアイテムやメールを復元する](https://go.microsoft.com/fwlink/?linkid=2103759)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="fc5fc-119">詳細については、「[Office 365 監査ログを検索して一般的なシナリオのトラブルシューティングを行う](https://go.microsoft.com/fwlink/?linkid=2103944)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="fc5fc-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>

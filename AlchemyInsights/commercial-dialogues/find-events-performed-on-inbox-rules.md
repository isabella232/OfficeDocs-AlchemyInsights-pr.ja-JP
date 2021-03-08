---
title: 受信トレイのルールで実行されたイベントを検索する
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484149"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="9eb10-102">受信トレイのルールで実行されたイベントを検索する</span><span class="sxs-lookup"><span data-stu-id="9eb10-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="9eb10-103">受信トレイのルールが作成、変更、または削除されると、イベントは監査ログに記録されます。</span><span class="sxs-lookup"><span data-stu-id="9eb10-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="9eb10-104">レビューする方法は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9eb10-104">Here's how to review them:</span></span>

1. <span data-ttu-id="9eb10-105">[Office 365 セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/p/?linkid=2077143)に移動します。</span><span class="sxs-lookup"><span data-stu-id="9eb10-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="9eb10-106">[検索] > [ログ検索の監査] を選択します。</span><span class="sxs-lookup"><span data-stu-id="9eb10-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="9eb10-107">監査を有効にする必要があるという通知が表示された場合は、先に進んで今すぐ有効にしてください。</span><span class="sxs-lookup"><span data-stu-id="9eb10-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="9eb10-108">この機能が有効になっていない場合、検索結果は前の日付からデータを取得できません。</span><span class="sxs-lookup"><span data-stu-id="9eb10-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="9eb10-109">[アクティビティ] フィールドを選択してExchange メールボックス アクティビティを見つけ、[新規] - [受信トレイのルール] [Outlook Web App から受信トレイの作成]ルールを選択します。 </span><span class="sxs-lookup"><span data-stu-id="9eb10-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="9eb10-110">完了したら、ウィンドウの外側をクリックして、[アクティビティ] ウィンドウを最小化します。</span><span class="sxs-lookup"><span data-stu-id="9eb10-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="9eb10-111">日付範囲を指定し、[ユーザー] フィールドで、調査するユーザーのユーザー名を選択します。</span><span class="sxs-lookup"><span data-stu-id="9eb10-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="9eb10-112">一度に複数のエントリを選択できます。</span><span class="sxs-lookup"><span data-stu-id="9eb10-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="9eb10-113">[検索] を選択します。</span><span class="sxs-lookup"><span data-stu-id="9eb10-113">Select Search.</span></span> <span data-ttu-id="9eb10-114">アクティビティは [結果] の下に表示されます。</span><span class="sxs-lookup"><span data-stu-id="9eb10-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="9eb10-115">詳細を表示するには、アクティビティを選択してから、[詳細情報] を選択します。</span><span class="sxs-lookup"><span data-stu-id="9eb10-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="9eb10-116">[パラメータ] セクションで、ルールの名前、設定された条件、およびルールが実行するアクションを確認できます。</span><span class="sxs-lookup"><span data-stu-id="9eb10-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="9eb10-117">詳細については、「Office 365 監査ログを検索して一般的なシナリオのトラブルシューティングを行う」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9eb10-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>
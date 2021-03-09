---
title: アーカイブ メールボックスへのメール メッセージの自動的な移動
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527953"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="aee14-102">アーカイブ メールボックスへのメール メッセージの自動的な移動</span><span class="sxs-lookup"><span data-stu-id="aee14-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="aee14-103">ここでは、ユーザーの古いメールを自動的にアーカイブ メールボックスに移動させるポリシーを設定する方法をご紹介します。</span><span class="sxs-lookup"><span data-stu-id="aee14-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="aee14-104">[**[セキュリティとコンプライアンス]**、](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **[データガバナンス]**、 > **[アーカイブ]** の順に移動して、アーカイブ メールボックスが有効になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="aee14-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="aee14-105">有効になっていない場合は、警告ボックスの **[無効化]** をクリックし、**[はい]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="aee14-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="aee14-106">[**[Exchange 管理センター]、[コンプライアンス管理]、[保持タグ]**](https://go.microsoft.com/fwlink/?linkid=2059104) の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="aee14-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="aee14-107">[+] アイコンを選択し、**メールボックス全体に自動適用** を選択します。</span><span class="sxs-lookup"><span data-stu-id="aee14-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="aee14-108">保持タグに名前を割り当て、**アーカイブに移動** を選択します。</span><span class="sxs-lookup"><span data-stu-id="aee14-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="aee14-109">保持期間には、90 日などの希望する期間を入力します。</span><span class="sxs-lookup"><span data-stu-id="aee14-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="aee14-110">**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="aee14-110">Click **Save**.</span></span>
5. <span data-ttu-id="aee14-111">これで、**アイテム保持ポリシー** を選択し、アイコンを選択して新しいポリシーを追加します。</span><span class="sxs-lookup"><span data-stu-id="aee14-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="aee14-112">保持ポリシーに名前を割り当て、クリックしてスクロールして、先ほど作成した保持タグを検出して追加します。</span><span class="sxs-lookup"><span data-stu-id="aee14-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="aee14-113">**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="aee14-113">Click **Save**.</span></span>
7. <span data-ttu-id="aee14-114">最後に、ユーザーのメールボックスにアイテム保持ポリシーを適用します。まだ Exchange 管理センターにいる場合は、**[受信者]**、 > **[メールボックス]** の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="aee14-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="aee14-115">ポリシーを適用したいユーザーをすべて選択し、**[編集]** を選択します (鉛筆のアイコン)。</span><span class="sxs-lookup"><span data-stu-id="aee14-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="aee14-116">ダイアログ ボックスで、**[メールボックスの機能]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="aee14-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="aee14-117">**[アイテム保持ポリシー]** で、今作成したポリシーを適用して、**[保存]** します。</span><span class="sxs-lookup"><span data-stu-id="aee14-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="aee14-118">すべてのユーザーにポリシーを適用する方法については、「[メールボックスにアイテム保持ポリシーを適用する](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)」参照してください。</span><span class="sxs-lookup"><span data-stu-id="aee14-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>

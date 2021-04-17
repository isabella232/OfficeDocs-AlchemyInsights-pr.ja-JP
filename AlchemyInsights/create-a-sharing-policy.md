---
title: 共有ポリシーを作成して、ユーザーが自分の予定表を組織外のユーザーと共有できるようにする
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
- "3800014"
- "898"
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816277"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="5edc1-102">共有ポリシーを作成して、ユーザーが自分の予定表を組織外のユーザーと共有できるようにする</span><span class="sxs-lookup"><span data-stu-id="5edc1-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="5edc1-103">Microsoft 365 管理センターのダッシュボードから、**[管理者]** > **[Exchange]** の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="5edc1-104">**[組織]** > **[共有]** の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="5edc1-105">リスト ビューの **[個別共有]** で、**[新規作成]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="5edc1-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="5edc1-106">**[共有ポリシーの新規作成]** で、**[ポリシー名]** ボックスに共有ポリシーのフレンドリ名を入力します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="5edc1-107">**[追加]** をクリックして、ポリシーの共有ルールを定義します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="5edc1-108">
            \*\*[共有ルール]\*\* で、次のいずれかのオプションを選択して、共有するドメインを指定します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="5edc1-109">**[すべてのドメインと共有]**</span><span class="sxs-lookup"><span data-stu-id="5edc1-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="5edc1-110">**[特定のドメインと共有]**</span><span class="sxs-lookup"><span data-stu-id="5edc1-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="5edc1-p101">
            **[特定のドメインと共有]\*\* を選択した場合は、共有するドメインの名前を入力します。この共有ポリシーに複数のドメインを入力する必要がある場合は、最初のドメインの設定値を保存してから、共有ルールを編集してさらにドメインを追加します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-p101">If you select **Sharing with a specific domain**, type the name of the domain you want to share with. If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="5edc1-113">共有できる情報を指定するには、**[予定表フォルダーを共有する]** チェック ボックスを選択してから、以下のいずれかのオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="5edc1-114">**[時刻のみを指定して予定表の空き時間情報にアクセス]**</span><span class="sxs-lookup"><span data-stu-id="5edc1-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="5edc1-115">**[時間、件名、場所を含む予定表の空き時間情報]**</span><span class="sxs-lookup"><span data-stu-id="5edc1-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="5edc1-116">**[時刻、件名、場所、役職などの予定表のすべての予定情報]**</span><span class="sxs-lookup"><span data-stu-id="5edc1-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="5edc1-117">共有ポリシーのルールを設定するには、**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="5edc1-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="5edc1-118">この共有ポリシーを組織内のすべてのユーザーの新しい既定の共有ポリシーに設定するには、 **[このポリシーを既定の共有ポリシーにする]** チェック ボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="5edc1-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="5edc1-119">**[保存]** をクリックして、共有ポリシーを作成します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="5edc1-120">**このトピックを完全に理解するためには、以下をお読みください。**</span><span class="sxs-lookup"><span data-stu-id="5edc1-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="5edc1-121">Exchange Online で共有ポリシーを作成する</span><span class="sxs-lookup"><span data-stu-id="5edc1-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="5edc1-122">Exchange Online で共有ポリシーをメールボックスに適用する</span><span class="sxs-lookup"><span data-stu-id="5edc1-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="5edc1-123">Exchange Online での共有ポリシーの変更、無効化、削除</span><span class="sxs-lookup"><span data-stu-id="5edc1-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)
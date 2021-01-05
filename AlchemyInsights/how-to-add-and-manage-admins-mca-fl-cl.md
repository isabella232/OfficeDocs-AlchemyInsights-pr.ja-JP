---
title: 管理者を追加および管理する方法 - MCA FL/CL
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692499"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="bacf1-102">管理者を追加および管理する方法 - MCA FL/CL</span><span class="sxs-lookup"><span data-stu-id="bacf1-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="bacf1-103">Microsoft 顧客契約 (MCA) の請求先アカウントを管理するために、必要なレベルのアクセス権を持つさまざまなロールを使用できます。</span><span class="sxs-lookup"><span data-stu-id="bacf1-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="bacf1-104">これらのロールは、リソースの制御に役立つ組み込みの Azure サービスのロールに追加されます。</span><span class="sxs-lookup"><span data-stu-id="bacf1-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="bacf1-105">**Azure ポータルに請求ロールを追加するには:**</span><span class="sxs-lookup"><span data-stu-id="bacf1-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="bacf1-106">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="bacf1-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="bacf1-107">*コストの管理と課金* で検索します。</span><span class="sxs-lookup"><span data-stu-id="bacf1-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="bacf1-108">アクセスを許可する請求先アカウント、請求プロファイル、請求書セクションなどの範囲でアクセス制御 (IAM) を選択します。</span><span class="sxs-lookup"><span data-stu-id="bacf1-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="bacf1-109">アクセス制御 (IAM) ページには、その範囲の各ロールに割り当てられているユーザーとグループが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="bacf1-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="bacf1-110">ユーザーにアクセスを許可するには、ページの上部で **[追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="bacf1-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="bacf1-111">*[ロール]* ドロップダウン リストで、ロールを選択します。</span><span class="sxs-lookup"><span data-stu-id="bacf1-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="bacf1-112">アクセスを許可するユーザーのメール アドレスを入力します。</span><span class="sxs-lookup"><span data-stu-id="bacf1-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="bacf1-113">**[保存]** を選択して、ロールを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="bacf1-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="bacf1-114">ユーザーのアクセスを削除するには、削除するロールが割り当てられているユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="bacf1-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="bacf1-115">**削除** を選択します。</span><span class="sxs-lookup"><span data-stu-id="bacf1-115">Select **Remove**.</span></span>

<span data-ttu-id="bacf1-116">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="bacf1-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="bacf1-117">請求ロールの定義</span><span class="sxs-lookup"><span data-stu-id="bacf1-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="bacf1-118">請求先アカウント ロールとタスク</span><span class="sxs-lookup"><span data-stu-id="bacf1-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="bacf1-119">MCA 請求先アカウントの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="bacf1-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="bacf1-120">Microsoft 顧客契約へのアクセス許可の確認</span><span class="sxs-lookup"><span data-stu-id="bacf1-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)

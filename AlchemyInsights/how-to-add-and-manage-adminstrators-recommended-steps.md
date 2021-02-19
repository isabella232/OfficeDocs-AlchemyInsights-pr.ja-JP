---
title: 管理者の追加および管理方法 - 推奨される手順
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755840"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="fa847-102">管理者の追加および管理方法 - 推奨される手順</span><span class="sxs-lookup"><span data-stu-id="fa847-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="fa847-103">お客様の問題の説明に基づいて、解決方法を見つけました。</span><span class="sxs-lookup"><span data-stu-id="fa847-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="fa847-104">ほとんどのお客様は、ドキュメントに従って、自分で問題を解決できました。</span><span class="sxs-lookup"><span data-stu-id="fa847-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="fa847-105">**サブスクリプション管理者または共同管理者を編集する**</span><span class="sxs-lookup"><span data-stu-id="fa847-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="fa847-106">アカウント管理者は両方の役割を編集できますが、サブスクリプション管理者は [Azure ポータル](https://ms.portal.azure.com/#home)でのみ共同管理者を変更できます。</span><span class="sxs-lookup"><span data-stu-id="fa847-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="fa847-107">Azure サブスクリプション管理者を追加または変更する</span><span class="sxs-lookup"><span data-stu-id="fa847-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="fa847-108">**サブスクリプション管理者または内部の共同管理者 (AIRS) を更新する**</span><span class="sxs-lookup"><span data-stu-id="fa847-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="fa847-109">サービス管理者または共同管理者は、次の手順を使用して、この操作をセルフサービスで実行できます。</span><span class="sxs-lookup"><span data-stu-id="fa847-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="fa847-110">[Azure ポータル](https://ms.portal.azure.com/#home)にログインし、左側のブレードの **[コスト管理と請求**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="fa847-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="fa847-111">サブスクリプションのある品目をクリックします。</span><span class="sxs-lookup"><span data-stu-id="fa847-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="fa847-112">サブスクリプションの概要が開きます。</span><span class="sxs-lookup"><span data-stu-id="fa847-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="fa847-113">**[サブスクリプション]** ブレードで、**[プロパティ]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="fa847-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="fa847-114">**[サービス管理者**] ボタンをクリックします。</span><span class="sxs-lookup"><span data-stu-id="fa847-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="fa847-115">サービス管理者として設定するユーザーのメールを入力し、**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="fa847-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="fa847-116">**共同管理者の追加/変更/削除**</span><span class="sxs-lookup"><span data-stu-id="fa847-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="fa847-117">サービス管理者として [Azure ポータル](https://ms.portal.azure.com/#home)にログインします。</span><span class="sxs-lookup"><span data-stu-id="fa847-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="fa847-118">[[サブスクリプション]](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) を開き、サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="fa847-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="fa847-119">(共同管理者は、サブスクリプション範囲でのみ割り当てることができます。)</span><span class="sxs-lookup"><span data-stu-id="fa847-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="fa847-120">**[アクセス制御 (IAM)]** > **[従来の管理者]** > **[追加]** > **[共同管理者の追加]** の順に移動し、**[共同管理者を追加]** ウィンドウを開きます ([共同管理者の追加] オプションが無効になっている場合は、権限がないことを示します)。</span><span class="sxs-lookup"><span data-stu-id="fa847-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="fa847-121">追加するユーザーを選択し、**[追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="fa847-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="fa847-122">**詳細情報:**</span><span class="sxs-lookup"><span data-stu-id="fa847-122">**Learn more:**</span></span>
- [<span data-ttu-id="fa847-123">共同管理者を追加する</span><span class="sxs-lookup"><span data-stu-id="fa847-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="fa847-124">共同管理者を削除する</span><span class="sxs-lookup"><span data-stu-id="fa847-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="fa847-125">サービス管理者を変更する</span><span class="sxs-lookup"><span data-stu-id="fa847-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="fa847-126">アカウント管理者を表示する</span><span class="sxs-lookup"><span data-stu-id="fa847-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="fa847-127">RBAC および Azure ポータルを使用してアクセスを管理する</span><span class="sxs-lookup"><span data-stu-id="fa847-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="fa847-128">**Azure Active Directory を使用してユーザーを追加/削除する**</span><span class="sxs-lookup"><span data-stu-id="fa847-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="fa847-129">Azure Active Directory (Azure AD) 組織から、新しいユーザーを追加したり、既存のユーザーを削除したりできます。</span><span class="sxs-lookup"><span data-stu-id="fa847-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="fa847-130">新しいユーザーを追加するには、組織のユーザー管理者として [Azure ポータル](https://ms.portal.azure.com/#home)にログインします。</span><span class="sxs-lookup"><span data-stu-id="fa847-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="fa847-131">**[Azure Active Directory]** を選択し、**[ユーザー]** を選択してから、**[新しいユーザー]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="fa847-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="fa847-132">**[ユーザー]** ページで、必要な情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="fa847-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="fa847-133">**[作成]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="fa847-133">Click **Create**.</span></span> <span data-ttu-id="fa847-134">ユーザーが作成され、Azure AD テナントに追加されます。</span><span class="sxs-lookup"><span data-stu-id="fa847-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="fa847-135">**詳細情報**:</span><span class="sxs-lookup"><span data-stu-id="fa847-135">**Learn more**:</span></span>

- [<span data-ttu-id="fa847-136">新しいユーザーを追加する</span><span class="sxs-lookup"><span data-stu-id="fa847-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="fa847-137">ユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="fa847-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="fa847-138">Azure Active Directory を使用してユーザーのプロファイル情報を追加または更新する</span><span class="sxs-lookup"><span data-stu-id="fa847-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="fa847-139">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="fa847-139">**Recommended documents**</span></span>

- [<span data-ttu-id="fa847-140">役割ベースのアクセス制御 (RBAC) とは</span><span class="sxs-lookup"><span data-stu-id="fa847-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="fa847-141">Azure のさまざまな役割を理解する</span><span class="sxs-lookup"><span data-stu-id="fa847-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="fa847-142">Azure Active Directory での管理者役割のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="fa847-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="fa847-143">チュートリアル: RBAC および Azure ポータルを使用してユーザーにアクセス権を付与する</span><span class="sxs-lookup"><span data-stu-id="fa847-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="fa847-144">Azure での RBAC のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="fa847-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="fa847-145">Azure 管理グループでリソースを編成する</span><span class="sxs-lookup"><span data-stu-id="fa847-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="fa847-146">メールで Azure 請求書のコピーを要求する方法</span><span class="sxs-lookup"><span data-stu-id="fa847-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/ja-JP/blog/azure-email-invoices/)
- [<span data-ttu-id="fa847-147">Azure でクレジット カードまたはデビット カードを追加、更新、または削除する方法</span><span class="sxs-lookup"><span data-stu-id="fa847-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="fa847-148">サブスクリプションの管理 (再アクティブ化/キャンセル/切り替え)</span><span class="sxs-lookup"><span data-stu-id="fa847-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)




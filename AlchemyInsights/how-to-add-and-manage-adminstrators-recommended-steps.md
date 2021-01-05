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
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2020
ms.locfileid: "49680454"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="0a165-102">管理者の追加および管理方法 - 推奨される手順</span><span class="sxs-lookup"><span data-stu-id="0a165-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="0a165-103">**サブスクリプション管理者または共同管理者を編集する**</span><span class="sxs-lookup"><span data-stu-id="0a165-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="0a165-104">アカウント管理者は両方の役割を編集できますが、サブスクリプション管理者は [Azure ポータル](https://ms.portal.azure.com/#home)でのみ共同管理者を変更できます。</span><span class="sxs-lookup"><span data-stu-id="0a165-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="0a165-105">Azure サブスクリプション管理者を追加または変更する</span><span class="sxs-lookup"><span data-stu-id="0a165-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="0a165-106">**サブスクリプション管理者または内部の共同管理者 (AIRS) を更新する**</span><span class="sxs-lookup"><span data-stu-id="0a165-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="0a165-107">サービス管理者または共同管理者は、次の手順を使用して、この操作をセルフサービスで実行できます。</span><span class="sxs-lookup"><span data-stu-id="0a165-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="0a165-108">[Azure ポータル](https://ms.portal.azure.com/#home)にログインし、左側のブレードの **[コスト管理と請求**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0a165-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="0a165-109">サブスクリプションのある品目をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0a165-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="0a165-110">サブスクリプションの概要が開きます。</span><span class="sxs-lookup"><span data-stu-id="0a165-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="0a165-111">**[サブスクリプション]** ブレードで、**[プロパティ]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0a165-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="0a165-112">**[サービス管理者**] ボタンをクリックします。</span><span class="sxs-lookup"><span data-stu-id="0a165-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="0a165-113">サービス管理者として設定するユーザーのメールを入力し、**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0a165-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="0a165-114">**共同管理者の追加/変更/削除**</span><span class="sxs-lookup"><span data-stu-id="0a165-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="0a165-115">サービス管理者として [Azure ポータル](https://ms.portal.azure.com/#home)にログインします。</span><span class="sxs-lookup"><span data-stu-id="0a165-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="0a165-116">[[サブスクリプション]](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) を開き、サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="0a165-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="0a165-117">(共同管理者は、サブスクリプション範囲でのみ割り当てることができます。)</span><span class="sxs-lookup"><span data-stu-id="0a165-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="0a165-118">**[アクセス制御 (IAM)]** > **[従来の管理者]** > **[追加]** > **[共同管理者の追加]** の順に移動し、**[共同管理者を追加]** ウィンドウを開きます ([共同管理者の追加] オプションが無効になっている場合は、権限がないことを示します)。</span><span class="sxs-lookup"><span data-stu-id="0a165-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="0a165-119">追加するユーザーを選択し、**[追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0a165-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="0a165-120">**詳細情報:**</span><span class="sxs-lookup"><span data-stu-id="0a165-120">**Learn more:**</span></span>
- [<span data-ttu-id="0a165-121">共同管理者を追加する</span><span class="sxs-lookup"><span data-stu-id="0a165-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="0a165-122">共同管理者を削除する</span><span class="sxs-lookup"><span data-stu-id="0a165-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="0a165-123">サービス管理者を変更する</span><span class="sxs-lookup"><span data-stu-id="0a165-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="0a165-124">アカウント管理者を表示する</span><span class="sxs-lookup"><span data-stu-id="0a165-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="0a165-125">RBAC および Azure ポータルを使用してアクセスを管理する</span><span class="sxs-lookup"><span data-stu-id="0a165-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="0a165-126">**Azure Active Directory を使用してユーザーを追加/削除する**</span><span class="sxs-lookup"><span data-stu-id="0a165-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="0a165-127">Azure Active Directory (Azure AD) 組織から、新しいユーザーを追加したり、既存のユーザーを削除したりできます。</span><span class="sxs-lookup"><span data-stu-id="0a165-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="0a165-128">新しいユーザーを追加するには、組織のユーザー管理者として [Azure ポータル](https://ms.portal.azure.com/#home)にログインします。</span><span class="sxs-lookup"><span data-stu-id="0a165-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="0a165-129">**[Azure Active Directory]** を選択し、**[ユーザー]** を選択してから、**[新しいユーザー]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0a165-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="0a165-130">**[ユーザー]** ページで、必要な情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="0a165-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="0a165-131">**[作成]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0a165-131">Click **Create**.</span></span> <span data-ttu-id="0a165-132">ユーザーが作成され、Azure AD テナントに追加されます。</span><span class="sxs-lookup"><span data-stu-id="0a165-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="0a165-133">**詳細情報**:</span><span class="sxs-lookup"><span data-stu-id="0a165-133">**Learn more**:</span></span>

- [<span data-ttu-id="0a165-134">新しいユーザーを追加する</span><span class="sxs-lookup"><span data-stu-id="0a165-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="0a165-135">ユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="0a165-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="0a165-136">Azure Active Directory を使用してユーザーのプロファイル情報を追加または更新する</span><span class="sxs-lookup"><span data-stu-id="0a165-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="0a165-137">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="0a165-137">**Recommended documents**</span></span>

- [<span data-ttu-id="0a165-138">役割ベースのアクセス制御 (RBAC) とは</span><span class="sxs-lookup"><span data-stu-id="0a165-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="0a165-139">Azure のさまざまな役割を理解する</span><span class="sxs-lookup"><span data-stu-id="0a165-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="0a165-140">Azure Active Directory での管理者役割のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a165-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="0a165-141">チュートリアル: RBAC および Azure ポータルを使用してユーザーにアクセス権を付与する</span><span class="sxs-lookup"><span data-stu-id="0a165-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="0a165-142">Azure での RBAC のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="0a165-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="0a165-143">Azure 管理グループでリソースを編成する</span><span class="sxs-lookup"><span data-stu-id="0a165-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="0a165-144">メールで Azure 請求書のコピーを要求する方法</span><span class="sxs-lookup"><span data-stu-id="0a165-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/ja-JP/blog/azure-email-invoices/)
- [<span data-ttu-id="0a165-145">Azure でクレジット カードまたはデビット カードを追加、更新、または削除する方法</span><span class="sxs-lookup"><span data-stu-id="0a165-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="0a165-146">サブスクリプションの管理 (再アクティブ化/キャンセル/切り替え)</span><span class="sxs-lookup"><span data-stu-id="0a165-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)




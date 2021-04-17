---
title: サポートされているサブスクリプションの種類
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
- "9003560"
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820687"
---
# <a name="supported-subscription-types"></a><span data-ttu-id="88b11-102">サポートされているサブスクリプションの種類</span><span class="sxs-lookup"><span data-stu-id="88b11-102">Supported subscription types</span></span>

<span data-ttu-id="88b11-103">詳細については、サポートされているサブスクリプションの種類を確認してください。</span><span class="sxs-lookup"><span data-stu-id="88b11-103">Please review the supported subscription types to proceed further.</span></span>

[<span data-ttu-id="88b11-104">サポートされているサブスクリプションの種類</span><span class="sxs-lookup"><span data-stu-id="88b11-104">Supported subscription types</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

<span data-ttu-id="88b11-105">**請求の所有権を譲渡する**</span><span class="sxs-lookup"><span data-stu-id="88b11-105">**Transfer billing ownership**</span></span>

<span data-ttu-id="88b11-106">転送するサブスクリプションを持つ請求先アカウントの[アカウント管理者](https://ms.portal.azure.com/)としての Azure ポータル</span><span class="sxs-lookup"><span data-stu-id="88b11-106">Azure portal as the [Account Admin](https://ms.portal.azure.com/) of the billing account that has the subscription you want to transfer</span></span>

- <span data-ttu-id="88b11-107">**コスト管理 + 請求** で検索します。</span><span class="sxs-lookup"><span data-stu-id="88b11-107">Search on **Cost Management + Billing**.</span></span> <span data-ttu-id="88b11-108">左側のウィンドウから **[サブスクリプション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="88b11-108">Select **Subscriptions** from left-pane.</span></span> <span data-ttu-id="88b11-109">アクセスに応じて、課金範囲を選択してから、**[サブスクリプション]** または **[Azure サブスクリプション]** を選択する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="88b11-109">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="88b11-110">転送するサブスクリプションの [請求所有権の転送] を選択します</span><span class="sxs-lookup"><span data-stu-id="88b11-110">Select Transfer billing ownership for the subscription you want to transfer</span></span>
- <span data-ttu-id="88b11-111">サブスクリプションの新しい所有者となるアカウントの請求管理者であるユーザーのメールアドレスを入力し、**[転送リクエストの送信]** を選択します</span><span class="sxs-lookup"><span data-stu-id="88b11-111">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="88b11-112">ユーザーには、譲渡要求を確認するための手順が記載されたメールが届きます。</span><span class="sxs-lookup"><span data-stu-id="88b11-112">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="88b11-113">譲渡要求を承認するには、ユーザーはメール内のリンクを選択し、指示に従います。</span><span class="sxs-lookup"><span data-stu-id="88b11-113">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="88b11-114">注: サブスクリプションの請求所有権を別の Azure AD テナントのユーザーのアカウントに譲渡すると、サブスクリプション内のリソースを管理するためのすべての[役割ベースのアクセス制御 (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) 割り当てが完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="88b11-114">Note: If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="88b11-115">新しい所有者のみが、サブスクリプション内のリソースを管理するためのアクセス権を持ちます。</span><span class="sxs-lookup"><span data-stu-id="88b11-115">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="88b11-116">詳細については、「[別のAzureADテナントのユーザーへのサブスクリプションの転送](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88b11-116">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="88b11-117">**サブスクリプションの所有権を譲渡する**</span><span class="sxs-lookup"><span data-stu-id="88b11-117">**Transfer Ownership of Subscription**</span></span>

<span data-ttu-id="88b11-118">サブスクリプション内のリソースを管理するためのサブスクリプション所有権転送の前提条件ロールベースアクセス (RBAC) は、アクセスを失います。</span><span class="sxs-lookup"><span data-stu-id="88b11-118">Subscription Ownership Transfer prerequisites role based access (RBAC) to manage resources in the subscription lose their access.</span></span> <span data-ttu-id="88b11-119">テナントへの既存のサブスクリプションの追加の詳細については、「[Azure ActiveDirectory への Azure サブスクリプションの関連付けまたは追加](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88b11-119">For more information about adding an existing subscription to a tenant, see [Associate or add an Azure subscription to Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

- <span data-ttu-id="88b11-120">現在の請求サイクルからの既存の未払い金額のサブスクリプション転送は、新しいアカウントの新しい支払い手段に転送されません。</span><span class="sxs-lookup"><span data-stu-id="88b11-120">Subscription Transfer with an existing outstanding amount from the current billing cycle will not be transferred to the new payment instrument in the new account.</span></span> <span data-ttu-id="88b11-121">新しいアカウントでユーザーが利用できる情報は、サブスクリプションの先月の費用のみになります。</span><span class="sxs-lookup"><span data-stu-id="88b11-121">The only information available to the users in new account is the last month's cost for your subscription.</span></span> <span data-ttu-id="88b11-122">それ以外の使用履歴と請求履歴は、サブスクリプションと一緒に転送されません。</span><span class="sxs-lookup"><span data-stu-id="88b11-122">The rest of the usage and billing history does not transfer with the subscription.</span></span>
- <span data-ttu-id="88b11-123">Enterprise Agreement (EA) サブスクリプションの請求所有権の譲渡は、現在Enterprise Agreement Portalでのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="88b11-123">Transfer billing ownership of Enterprise Agreement (EA) subscriptions is currently supported in the Enterprise Agreement Portal only</span></span>
- <span data-ttu-id="88b11-124">Visual Studio、BizSpark、Microsoft パートナーネットワークなどのクレジット指向のサブスクリプションを新しいユーザーに転送するには、転送要求を受け入れるために Visual Studio / Microsoft パートナーネットワークライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="88b11-124">Transferring a credit-oriented subscription like Visual Studio, BizSpark, Microsoft Partner Network to a new user requires to have a Visual Studio/Microsoft partner network license to accept the transfer request</span></span>
- <span data-ttu-id="88b11-125">仮想マシン、ディスク、Web サイトなどのすべてのリソースは、新しいアカウントに正常に転送されます。</span><span class="sxs-lookup"><span data-stu-id="88b11-125">All resources like Virtual Machines, disks, and websites transfer to the new account successfully.</span></span> <span data-ttu-id="88b11-126">テナント間のサブスクリプション転送では、次のリソースが影響を受ける可能性があります。</span><span class="sxs-lookup"><span data-stu-id="88b11-126">The following resources could be affected in a cross-tenant subscription transfer:</span></span>

<span data-ttu-id="88b11-127">**Azure AD Domain Services**</span><span class="sxs-lookup"><span data-stu-id="88b11-127">**Azure AD Domain Services**</span></span>

<span data-ttu-id="88b11-128">Azure Key Vault</span><span class="sxs-lookup"><span data-stu-id="88b11-128">Azure Key Vaults</span></span>

- <span data-ttu-id="88b11-129">特に顧客が AzureActive Directory 関連の認証を使用している場合、[SQL 関連のユーザーとデータベース](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support)が影響を受ける可能性があります</span><span class="sxs-lookup"><span data-stu-id="88b11-129">[SQL related users and databases](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) could be impacted, especially if the customer uses an Azure Active Directory related authentication</span></span>
- <span data-ttu-id="88b11-130">Azure Active Directory 認証で構成された **App Services** が影響を受ける可能性があります</span><span class="sxs-lookup"><span data-stu-id="88b11-130">**App Services** configured with Azure Active Directory authentication could be impacted</span></span>
- <span data-ttu-id="88b11-131">Azure サブスクリプションに接続されている **Visual Studio Team** Services アカウントは、接続されている Azure サブスクリプションがキャンセルされると一時的にアクセスできなくなる場合があります</span><span class="sxs-lookup"><span data-stu-id="88b11-131">**Visual Studio Team** Services accounts connected to Azure subscriptions may temporarily lose access when the connected Azure subscription is cancelled</span></span>

<span data-ttu-id="88b11-132">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="88b11-132">**Recommended Documents**</span></span>

<span data-ttu-id="88b11-133">請求の所有権を承諾した後の手順:</span><span class="sxs-lookup"><span data-stu-id="88b11-133">Steps after accepting billing ownership:</span></span>

- <span data-ttu-id="88b11-134">請求の所有権を保持し、サブスクリプションのタイプを変更するには、次を参照してください: [Azureサブスクリプションを別のプランに切り替える](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="88b11-134">To retain billing ownership, but change the type of your subscription, refer: [Switch your Azure subscription to another offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- [<span data-ttu-id="88b11-135">Visual Studio、Microsoft Partner Network (MPN)、および Pay as you go Dev / Test サブスクリプションの移行</span><span class="sxs-lookup"><span data-stu-id="88b11-135">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="88b11-136">Enterprise Agreement (EA) サブスクリプションの請求所有権の移転</span><span class="sxs-lookup"><span data-stu-id="88b11-136">Transfer billing ownership of Enterprise Agreement (EA) subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [<span data-ttu-id="88b11-137">所有権の譲渡についての FAQ</span><span class="sxs-lookup"><span data-stu-id="88b11-137">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="88b11-138">所有権の移転に関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="88b11-138">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
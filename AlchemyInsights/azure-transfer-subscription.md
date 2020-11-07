---
title: Azure の請求の所有権を譲渡する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922250"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="338bb-102">Azure の請求の所有権を譲渡する</span><span class="sxs-lookup"><span data-stu-id="338bb-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="338bb-103">譲渡するサブスクリプションを所有している請求アカウントの管理者として [Azure ポータル](https://portal.azure.com/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="338bb-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="338bb-104">自分が管理者なのかどうかがわからない場合、または管理者を決定する必要がある場合には、「[Determine account billing administrator (アカウントの課金管理者を決定する)](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="338bb-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="338bb-105">**コスト管理 + 請求** で検索します。</span><span class="sxs-lookup"><span data-stu-id="338bb-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="338bb-106">左側のウィンドウから **[サブスクリプション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="338bb-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="338bb-107">アクセスに応じて、課金範囲を選択してから **[サブスクリプション]** または **[Azure サブスクリプション]** を選択する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="338bb-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="338bb-108">譲渡するサブスクリプションの **[請求の所有権を譲渡する]** を選択します</span><span class="sxs-lookup"><span data-stu-id="338bb-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="338bb-109">サブスクリプションの新しい所有者となるアカウントの請求管理者であるユーザーのメールアドレスを入力し、 **[転送リクエストの送信]** を選択します</span><span class="sxs-lookup"><span data-stu-id="338bb-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="338bb-110">ユーザーには、転送リクエストを確認するための手順が記載されたメールが届きます。</span><span class="sxs-lookup"><span data-stu-id="338bb-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="338bb-111">転送要求を承認するには、ユーザーはメール内のリンクを選択し、指示に従います。</span><span class="sxs-lookup"><span data-stu-id="338bb-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="338bb-112">**注** : サブスクリプションの請求所有権を別の Azure AD テナントのユーザーのアカウントに譲渡すると、サブスクリプション内のリソースを管理するためのすべての[役割ベースのアクセス制御 (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) の割り当てが完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="338bb-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="338bb-113">新しい所有者のみが、サブスクリプション内のリソースを管理するためのアクセス権を持ちます。</span><span class="sxs-lookup"><span data-stu-id="338bb-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="338bb-114">詳細については、「[別のAzureADテナントのユーザーへのサブスクリプションの転送](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="338bb-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="338bb-115">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="338bb-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="338bb-116">Azure サブスクリプションの請求所有権を別のアカウントに譲渡する</span><span class="sxs-lookup"><span data-stu-id="338bb-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="338bb-117">Azure サブスクリプションの請求所有権の譲渡について</span><span class="sxs-lookup"><span data-stu-id="338bb-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="338bb-118">Visual Studio、Microsoft Partner Network (MPN)、Pay as you go 開発/テスト サブスクリプションの譲渡</span><span class="sxs-lookup"><span data-stu-id="338bb-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="338bb-119">所有権の譲渡についての FAQ</span><span class="sxs-lookup"><span data-stu-id="338bb-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="338bb-120">所有権の移転に関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="338bb-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)

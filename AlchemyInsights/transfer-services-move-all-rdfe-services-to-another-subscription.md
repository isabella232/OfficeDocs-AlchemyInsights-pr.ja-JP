---
title: サービスの転送 - すべての RDFE サービスを別のサブスクリプションに移動する
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692487"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="d6e5f-102">サービスの転送 - すべての RDFE サービスを別のサブスクリプションに移動する</span><span class="sxs-lookup"><span data-stu-id="d6e5f-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="d6e5f-103">**リソースを移動する**</span><span class="sxs-lookup"><span data-stu-id="d6e5f-103">**Move resources**</span></span>

<span data-ttu-id="d6e5f-104">Azure portal、Azure PowerShell、Azure CLI、または REST API を使用してリソースを移動すると、Azure リソースを同じサブスクリプションの中の別の Azure サブスクリプションまたはリソース グループに移動できます。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="d6e5f-105">リソースを移動する前に、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="d6e5f-106">リソースの移動前のチェック リスト</span><span class="sxs-lookup"><span data-stu-id="d6e5f-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="d6e5f-107">移動可能なサービス</span><span class="sxs-lookup"><span data-stu-id="d6e5f-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="d6e5f-108">移動の検証方法</span><span class="sxs-lookup"><span data-stu-id="d6e5f-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="d6e5f-109">サービスの移動ガイダンス</span><span class="sxs-lookup"><span data-stu-id="d6e5f-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="d6e5f-110">既存のリソースを別のリソース グループまたはサブスクリプションに移動するには、次を使用できます。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="d6e5f-111">Azure portal</span><span class="sxs-lookup"><span data-stu-id="d6e5f-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="d6e5f-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="d6e5f-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="d6e5f-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="d6e5f-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="d6e5f-114">REST API</span><span class="sxs-lookup"><span data-stu-id="d6e5f-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="d6e5f-115">チュートリアル: [既存のリソースを別のリソース グループまたはサブスクリプションに移動する](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="d6e5f-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="d6e5f-116">**Azure Resource Manager でエラーをトラブルシューティングする**</span><span class="sxs-lookup"><span data-stu-id="d6e5f-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="d6e5f-117">以下の記事を参照して、いくつかの一般的な Azure 展開エラーについて学習し、それらを解決するための情報を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="d6e5f-118">展開エラーのエラー コードが見つからない場合は、[エラーコードの検索](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="d6e5f-119">展開エラーのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="d6e5f-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="d6e5f-120">既存のリソースを新しいリソース グループまたはサブスクリプションに移動する際のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="d6e5f-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="d6e5f-121">無料から従量課金制への切り替えなど、Azure サブスクリプションをアップグレードする場合は、サブスクリプションを変換する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="d6e5f-122">無料試用版をアップグレードするには、「[無料試用版のアップグレードまたは Microsoft Imagine Azure サブスクリプションを従量課金制にアップグレードする](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="d6e5f-123">従量課金制のアカウントを変更するには、「[Azure従量課金制のサブスクリプションを別のオファーに変更する](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="d6e5f-124">**Azure サブスクリプションを Azure Active Directoryテ ナントに追加または関連付けするには、以下の操作を行います。**</span><span class="sxs-lookup"><span data-stu-id="d6e5f-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="d6e5f-125">サインインして、[Azure portal の [サブスクリプション] ページ](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)から使用するサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="d6e5f-126">**[ディレクトリの変更]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="d6e5f-127">表示される警告を確認してから、**[変更]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="d6e5f-128">サブスクリプションのディレクトリが変更され、成功メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="d6e5f-129">*ディレクトリ* スイッチャーを使用して、新しいディレクトリに移動します。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="d6e5f-130">すべてが正しく表示されるまでに最大 10 分かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="d6e5f-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="d6e5f-131">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="d6e5f-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="d6e5f-132">Azure サブスクリプションの請求所有権の譲渡について</span><span class="sxs-lookup"><span data-stu-id="d6e5f-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="d6e5f-133">既存のリソースを新しいリソース グループまたはサブスクリプションに移動する</span><span class="sxs-lookup"><span data-stu-id="d6e5f-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="d6e5f-134">Azure portal を使用してリソースを管理する</span><span class="sxs-lookup"><span data-stu-id="d6e5f-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)

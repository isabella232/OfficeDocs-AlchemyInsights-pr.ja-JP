---
title: 予約インスタンスの購入
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
- "9003552"
- "6816"
ms.openlocfilehash: 4e42d4a3d7c3cb3a08264fac768606319ffe0043
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809912"
---
# <a name="questions-before-purchase"></a><span data-ttu-id="6ec7c-102">購入前の質問</span><span class="sxs-lookup"><span data-stu-id="6ec7c-102">Questions before purchase</span></span>

<span data-ttu-id="6ec7c-103">**既存のリソースに対して予約割引を適用するには、どうすればいいですか?**</span><span class="sxs-lookup"><span data-stu-id="6ec7c-103">**How is reservation discount applied to existing resources?**</span></span>  
<span data-ttu-id="6ec7c-104">予約特典は、予約 SKU、地域、および範囲と一致する既存のリソースに自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="6ec7c-104">Reservation benefit automatically applies to existing resources that match the reservation SKU, region and scope.</span></span> <span data-ttu-id="6ec7c-105">リソースに対する予約のタグ付けはありません。</span><span class="sxs-lookup"><span data-stu-id="6ec7c-105">There is no tagging of a reservation to a resource.</span></span> [<span data-ttu-id="6ec7c-106">詳細情報</span><span class="sxs-lookup"><span data-stu-id="6ec7c-106">Learn more</span></span>](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support#how-reservation-discount-is-applied) 

<span data-ttu-id="6ec7c-107">**どの仮想マシンを購入すればいいですか?**</span><span class="sxs-lookup"><span data-stu-id="6ec7c-107">**Which VM size should I buy?**</span></span>  
<span data-ttu-id="6ec7c-108">こちらの「[購入前に適正な仮想マシンのサイズを判断する](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?toc=/azure/billing/TOC.json&WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)」の記事を読んでください。</span><span class="sxs-lookup"><span data-stu-id="6ec7c-108">Read this article: [Determine the right VM size before you buy](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?toc=/azure/billing/TOC.json&WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)</span></span>

<span data-ttu-id="6ec7c-109">**SQL の予約容量を購入する方法について、質問があります。**</span><span class="sxs-lookup"><span data-stu-id="6ec7c-109">**Questions on how to buy SQL reserved capacity?**</span></span>  
<span data-ttu-id="6ec7c-110">こちらの「[SQL データベースの予約容量を購入する](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity?toc=/azure/billing/TOC.json&WT.mc_id=Portal-Microsoft_Azure_Support#buy-sql-database-reserved-capacity)」の記事を読んでください。</span><span class="sxs-lookup"><span data-stu-id="6ec7c-110">Read this article: [Buy SQL Database reserved capacity](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity?toc=/azure/billing/TOC.json&WT.mc_id=Portal-Microsoft_Azure_Support#buy-sql-database-reserved-capacity)</span></span>

<span data-ttu-id="6ec7c-111">**間接的な EA カスタマーなのですが、パートナーがいないと購入できませんか?**</span><span class="sxs-lookup"><span data-stu-id="6ec7c-111">**I am in Indirect EA customer, do I need my partner to purchase?**</span></span>  
<span data-ttu-id="6ec7c-112">いいえ。 EA サブスクリプションの所有者であれば、RI を購入できます。</span><span class="sxs-lookup"><span data-stu-id="6ec7c-112">No, you can purchase the RI if you an owner on an EA subscription.</span></span>

<span data-ttu-id="6ec7c-113">**RI の購入は金額コミットメントから控除されますか?**</span><span class="sxs-lookup"><span data-stu-id="6ec7c-113">**Does RI purchase deduct from monetary commitment?**</span></span>  
<span data-ttu-id="6ec7c-114">はい。</span><span class="sxs-lookup"><span data-stu-id="6ec7c-114">Yes.</span></span> <span data-ttu-id="6ec7c-115">金額コミットメントが十分でない場合は、使用可能な金額コミットメントを超過する金額の料金の請求が行われます。</span><span class="sxs-lookup"><span data-stu-id="6ec7c-115">If you don’t have enough monetary commitment, you will get an overage invoice for the amount that exceeds the available monetary commitment.</span></span>

<span data-ttu-id="6ec7c-116">**予約インスタンスは Windows VM か SQL IP コストのどちらに適用されますか?**</span><span class="sxs-lookup"><span data-stu-id="6ec7c-116">**How does reserved instance apply to Windows VMs or to my SQL IP costs?**</span></span>  
<span data-ttu-id="6ec7c-117">予約インスタンスの割引は、コンピューティングの使用状況にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="6ec7c-117">The reserved instance discount only applies to the compute usage.</span></span> <span data-ttu-id="6ec7c-118">Windows IP コストまたは SQL IP コストは個別に課金され、RI 割引は取得できません。</span><span class="sxs-lookup"><span data-stu-id="6ec7c-118">Windows IP or SQL IP costs will be charged separately and don’t get RI discount.</span></span> [<span data-ttu-id="6ec7c-119">Azure Reserved VM Instances を含まないソフトウェア コスト</span><span class="sxs-lookup"><span data-stu-id="6ec7c-119">Software costs not included with Azure Reserved VM Instances</span></span>](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs?WT.mc_id=Portal-Microsoft_Azure_Support)  
      
<span data-ttu-id="6ec7c-120">**予約インスタンスの購入に対する課金**</span><span class="sxs-lookup"><span data-stu-id="6ec7c-120">**Billing for Reserved Instance purchase**</span></span>  
      
<span data-ttu-id="6ec7c-121">予約インスタンス購入は、購入時点で選択したサブスクリプションに紐付いた支払方法で課金されます。</span><span class="sxs-lookup"><span data-stu-id="6ec7c-121">The reserved instance purchase is charged to the payment method tied to the subscription that you select at the time of purchase.</span></span> <span data-ttu-id="6ec7c-122">サブスクリプションの種類は、エンタープライズ契約 (オファー番号: MS-AZR-0017P)、従量課金制 (オファー番号: MS-AZR-0003P)、Microsoft 顧客契約、または CSP にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ec7c-122">The subscription type must be an enterprise agreement (offer number: MS-AZR-0017P), Pay-As-You-Go (offer number: MS-AZR-0003P), Microsoft Customer Agreement or CSP.</span></span>

-   <span data-ttu-id="6ec7c-123">エンタープライズ サブスクリプションでは、料金が登録した金額コミットメント残高から控除されるか、または過剰として請求されます</span><span class="sxs-lookup"><span data-stu-id="6ec7c-123">For an enterprise subscription, the charges are deducted from the enrollment's monetary commitment balance or charged as overage</span></span>
-   <span data-ttu-id="6ec7c-124">従量課金制サブスクリプションを利用する場合は、サブスクリプションのクレジットカードまたは請求書による支払い方法で料金が請求されます</span><span class="sxs-lookup"><span data-stu-id="6ec7c-124">For Pay-As-You-Go subscription, the charges are billed to the credit card or invoice payment method on the subscription</span></span>

<span data-ttu-id="6ec7c-125">**サービス プランの購入は、次のとおりです。**</span><span class="sxs-lookup"><span data-stu-id="6ec7c-125">**Buy a service plan:**</span></span>

-   [<span data-ttu-id="6ec7c-126">Cosmos DB 予約容量に対する前払い</span><span class="sxs-lookup"><span data-stu-id="6ec7c-126">Prepay for Cosmos DB reserved capacity</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity?WT.mc_id=Portal-Microsoft_Azure_Support)
-   [<span data-ttu-id="6ec7c-127">Azure SQL Database 予約容量を使用して SQL データベース コンピューティング リソースへの前払いを行う</span><span class="sxs-lookup"><span data-stu-id="6ec7c-127">Prepay for SQL Database compute resources with Azure SQL Database reserved capacity</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity?WT.mc_id=Portal-Microsoft_Azure_Support)
-   [<span data-ttu-id="6ec7c-128">Azure Reserved VM Instances を使用して仮想マシンへの前払いを行う</span><span class="sxs-lookup"><span data-stu-id="6ec7c-128">Prepay for Virtual Machines with Azure Reserved VM Instances</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="6ec7c-129">**ソフトウェア プランの購入は、次のとおりです。**</span><span class="sxs-lookup"><span data-stu-id="6ec7c-129">**Buy a software plan:**</span></span>

-   [<span data-ttu-id="6ec7c-130">Azure 予約から Red Hat ソフトウェア プランへの前払いを行う</span><span class="sxs-lookup"><span data-stu-id="6ec7c-130">Prepay for Red Hat software plans from Azure Reservations</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-rhel-software-charges?WT.mc_id=Portal-Microsoft_Azure_Support)
-   [<span data-ttu-id="6ec7c-131">Azure 予約から SUSE ソフトウェア プランへの前払いを行う</span><span class="sxs-lookup"><span data-stu-id="6ec7c-131">Prepay for SUSE software plans from Azure Reservations</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges?WT.mc_id=Portal-Microsoft_Azure_Support)
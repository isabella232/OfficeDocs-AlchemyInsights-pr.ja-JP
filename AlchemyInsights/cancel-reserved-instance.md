---
title: 予約のキャンセル
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
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808218"
---
# <a name="cancelling-reservation"></a><span data-ttu-id="14369-102">予約のキャンセル</span><span class="sxs-lookup"><span data-stu-id="14369-102">Cancelling Reservation</span></span>

- <span data-ttu-id="14369-103">**セルフサービス**: [Azure ポータル](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)を使用して、予約済みインスタンスを自分でキャンセルまたは交換できます。</span><span class="sxs-lookup"><span data-stu-id="14369-103">**Self-service:** You can cancel or exchange a reserved instance yourself using [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="14369-104">予約を選択し、[返金] または [交換] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="14369-104">Select the reservation and click on refund or exchange.</span></span> <span data-ttu-id="14369-105">交換または返金するには、予約注文の所有者アクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="14369-105">Note that you must have owner access on the Reservation Order to exchange or refund.</span></span> <span data-ttu-id="14369-106">予約のみにアクセスしても、返金や交換はできません。</span><span class="sxs-lookup"><span data-stu-id="14369-106">Access to only the Reservation will not let you proceed with refund or exchange.</span></span> <span data-ttu-id="14369-107">予約注文の所有者に、予約注文へのアクセスを許可するよう依頼してください</span><span class="sxs-lookup"><span data-stu-id="14369-107">Ask the Reservation Order owner to give you owner access to the Reservation Order</span></span>
- <span data-ttu-id="14369-108">**交換ポリシー:** 予約を同じタイプの別の予約と交換できます。予約交換に **ペナルティはありません**。</span><span class="sxs-lookup"><span data-stu-id="14369-108">**Exchange policy:** You can exchange a reservation for another reservation of the same type – there are **no penalties** on reservation exchange.</span></span> <span data-ttu-id="14369-109">新規予約の合計コミットメントは、交換された予約の払い戻し額と将来の毎月の支払い (該当する場合) の合計よりも大きくする必要があります</span><span class="sxs-lookup"><span data-stu-id="14369-109">The total commitment with new reservation should be greater than the sum of exchanged reservation’s refund amount and the future monthly payments (if applicable)</span></span>
- <span data-ttu-id="14369-110">**払い戻しポリシー**: 払い戻しとキャンセルされた将来の支払いの合計は、12 か月のローリングウィンドウで 50,000 米ドルを超えることはできません。</span><span class="sxs-lookup"><span data-stu-id="14369-110">**Refund policy:** Sum of refund and the cancelled future payments cannot exceed $50,000 USD in a 12-month rolling window.</span></span> <span data-ttu-id="14369-111">**現在、払い戻しにはペナルティを課していません** が、将来の払い戻しに課す可能性があります</span><span class="sxs-lookup"><span data-stu-id="14369-111">We are **currently not charging any penalty** on refunds but could charge it on future refunds</span></span>  
    <span data-ttu-id="14369-112">**例外:** セルフサービスの交換およびキャンセル機能は、米国政府のエンタープライズ契約のお客様にはご利用いただけません</span><span class="sxs-lookup"><span data-stu-id="14369-112">**Exceptions:** Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers</span></span>
- <span data-ttu-id="14369-113">**API / PS / CLI** サポートは、[Azure予約のキャンセルと払い戻し、セルフサービス交換と払い戻し](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)には利用できません。</span><span class="sxs-lookup"><span data-stu-id="14369-113">**API / PS / CLI** support is not available for cancellation and refunds [Self-service exchanges and refunds for Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- <span data-ttu-id="14369-114">セルフサービスの交換およびキャンセル機能は、米国政府のエンタープライズ契約のお客様にはご利用いただけません。</span><span class="sxs-lookup"><span data-stu-id="14369-114">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="14369-115">Pay-As-You-Go や CSP などの他の米国政府のサブスクリプション タイプがサポートされています</span><span class="sxs-lookup"><span data-stu-id="14369-115">Other US Government subscription types including Pay-As-You-Go and CSP are supported</span></span>

<span data-ttu-id="14369-116">詳細情報: [返品および交換トランザクションの処理方法](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)</span><span class="sxs-lookup"><span data-stu-id="14369-116">Learn more : [How return and exchange transactions are processed](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)</span></span>  
<span data-ttu-id="14369-117">詳細情報: [交換および返金ポリシー](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)</span><span class="sxs-lookup"><span data-stu-id="14369-117">Learn more : [Exchange and Refund policies](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)</span></span>  
<span data-ttu-id="14369-118">その他の質問: [予約済みインスタンスのドキュメントにアクセスする](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="14369-118">Other questions: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="14369-119">**既存の予約済みインスタンスを交換する (セルフサービス)**</span><span class="sxs-lookup"><span data-stu-id="14369-119">**Exchange an existing reserved instance (Self-service)**</span></span>

<span data-ttu-id="14369-120">同じタイプの別の予約と交換できます。</span><span class="sxs-lookup"><span data-stu-id="14369-120">You can exchange a reservation for another reservation of the same type.</span></span> <span data-ttu-id="14369-121">予約が不要になった場合は、年間最大 50,000 米ドルまで返金することもできます。</span><span class="sxs-lookup"><span data-stu-id="14369-121">You can also refund a reservation, up to $50,000 USD per year, if you no longer need it.</span></span> <span data-ttu-id="14369-122">セルフサービスの交換およびキャンセル機能は、米国政府のエンタープライズ契約のお客様にはご利用いただけません。</span><span class="sxs-lookup"><span data-stu-id="14369-122">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="14369-123">Pay-As-You-Go や CSP など、他の米国政府のサブスクリプション タイプがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="14369-123">Other US Government subscription types including Pay-As-You-Go and CSP are supported.</span></span> <span data-ttu-id="14369-124">既存の予約を交換または返金するには、予約注文の所有者アクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="14369-124">You must have owner access on the Reservation Order to exchange or refund an existing reservation.</span></span>

<span data-ttu-id="14369-125">トランザクションを完了する方法については、次の手順を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14369-125">The following steps will guide on the procedure to complete the transaction</span></span>

1. <span data-ttu-id="14369-126">[Azure ポータル](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="14369-126">Log in to your [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="14369-127">返金する予約を選択し、**[交換]** をクリックします</span><span class="sxs-lookup"><span data-stu-id="14369-127">Select the reservations that you want to refund and click **Exchange**</span></span>
2. <span data-ttu-id="14369-128">購入する VM 製品を選び、数量を入力します。</span><span class="sxs-lookup"><span data-stu-id="14369-128">Select the VM product that you want to purchase and type a quantity.</span></span> <span data-ttu-id="14369-129">新規購入の合計が返品の合計よりも多いことを確認し、[購入する前に適切なサイズを決定](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)します</span><span class="sxs-lookup"><span data-stu-id="14369-129">Make sure that the new purchase total is more than the return total [Determine the right size before you purchase](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)</span></span>
3. <span data-ttu-id="14369-130">トランザクションを確認して完了します</span><span class="sxs-lookup"><span data-stu-id="14369-130">Review and complete the transaction</span></span>

<span data-ttu-id="14369-131">**予約済みインスタンスの払い戻し**</span><span class="sxs-lookup"><span data-stu-id="14369-131">**Refund for a reserved instance**</span></span>

<span data-ttu-id="14369-132">予約を返金するには、**[予約の詳細]** に移動し、**[返金]** をクリックします</span><span class="sxs-lookup"><span data-stu-id="14369-132">To refund a reservation, go to **Reservation Details** and click **Refund**</span></span>

<span data-ttu-id="14369-133">**比例配分された払い戻し:**</span><span class="sxs-lookup"><span data-stu-id="14369-133">**Pro-rated refund:**</span></span>

<span data-ttu-id="14369-134">**払い戻しと交換の比例配分と最小要件の例**</span><span class="sxs-lookup"><span data-stu-id="14369-134">**Pro-ration and minimum requirement examples for refund and exchange**</span></span>  
<span data-ttu-id="14369-135">事前予約の例:</span><span class="sxs-lookup"><span data-stu-id="14369-135">Upfront reservation example:</span></span>

- <span data-ttu-id="14369-136">1 月 1 日に 1 年間の RI を 120 ドルで購入します。</span><span class="sxs-lookup"><span data-stu-id="14369-136">You purchase a one-year term RI for $120 on January 1</span></span>
- <span data-ttu-id="14369-137">4 月 7 日に、この予約の払い戻しまたは交換を希望します</span><span class="sxs-lookup"><span data-stu-id="14369-137">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="14369-138">予約は 97 日間有効であるため、(1 - 97 ÷ 365) × 120 ドルが返金されます。</span><span class="sxs-lookup"><span data-stu-id="14369-138">Since the reservation has been live for 97 days, you will get (1-97/365) \* $120 back.</span></span> <span data-ttu-id="14369-139">(およそ 88.1 ドルです)。</span><span class="sxs-lookup"><span data-stu-id="14369-139">(i.e. $88.1).</span></span> <span data-ttu-id="14369-140">現在、払い戻しに対するペナルティはありません</span><span class="sxs-lookup"><span data-stu-id="14369-140">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="14369-141">交換する場合、新規購入は 88.1 ドルを超える必要があります</span><span class="sxs-lookup"><span data-stu-id="14369-141">If exchanging, your new purchase should be greater than $88.1</span></span>
- <span data-ttu-id="14369-142">現在、払い戻しにペナルティはありません</span><span class="sxs-lookup"><span data-stu-id="14369-142">There is no penalty on refunds currently</span></span>

<span data-ttu-id="14369-143">**請求プランの予約例:**</span><span class="sxs-lookup"><span data-stu-id="14369-143">**Billing plan reservation example:**</span></span>

- <span data-ttu-id="14369-144">1 月 1 日に 1 年間の RI を月額 10 ドルで購入します。</span><span class="sxs-lookup"><span data-stu-id="14369-144">You purchase a one-year term RI for $10 per month</span></span>
- <span data-ttu-id="14369-145">4 月 7 日に、この予約の払い戻しまたは交換を希望します</span><span class="sxs-lookup"><span data-stu-id="14369-145">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="14369-146">最後に支払いが 7 日間発生したので、(1 - 7 ÷ 31) × 10 ドルが返金されます。</span><span class="sxs-lookup"><span data-stu-id="14369-146">Since the last payment happened 7 days, you will get (1-7/31) \* $10 back.</span></span> <span data-ttu-id="14369-147">(およそ 7.74 ドルです)。</span><span class="sxs-lookup"><span data-stu-id="14369-147">(i.e. $7.74)</span></span>
- <span data-ttu-id="14369-148">キャンセルされる将来の支払いは 80 ドルです。</span><span class="sxs-lookup"><span data-stu-id="14369-148">The future payments cancelled are $ 80.</span></span> <span data-ttu-id="14369-149">現在、払い戻しに対するペナルティはありません</span><span class="sxs-lookup"><span data-stu-id="14369-149">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="14369-150">このキャンセルにより、50,000 ドルの払い戻し限度額から 87.74 ドルが差し引かれます。</span><span class="sxs-lookup"><span data-stu-id="14369-150">This cancellation will deduct $87.74 from you’re the $50,000 refund limit</span></span>
- <span data-ttu-id="14369-151">交換する場合、新規購入は 87.74 ドルを超える必要があります</span><span class="sxs-lookup"><span data-stu-id="14369-151">If exchanging, the total value of new purchase should be greater than $87.74</span></span>

<span data-ttu-id="14369-152">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="14369-152">**Recommended Documents**</span></span>

- [<span data-ttu-id="14369-153">返品および交換トランザクションの処理方法</span><span class="sxs-lookup"><span data-stu-id="14369-153">How return and exchange transactions are processed</span></span>](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [<span data-ttu-id="14369-154">交換および返金ポリシー</span><span class="sxs-lookup"><span data-stu-id="14369-154">Exchange and Refund policies</span></span>](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)
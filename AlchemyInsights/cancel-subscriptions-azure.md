---
title: Azure でのサブスクリプションのキャンセル
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003797"
- "6786"
ms.openlocfilehash: 83fab49ccafd23352fe28569289a709a198fd402
ms.sourcegitcommit: 80a36e6447953b3f65e45c05607dbfc585fbf8b0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/21/2021
ms.locfileid: "51936159"
---
# <a name="cancel-subscription"></a><span data-ttu-id="c1fbf-102">サブスクリプションのキャンセル</span><span class="sxs-lookup"><span data-stu-id="c1fbf-102">Cancel Subscription</span></span>

<span data-ttu-id="c1fbf-103">Azure サブスクリプションが不要になった場合は、Azure portal でキャンセルできます。</span><span class="sxs-lookup"><span data-stu-id="c1fbf-103">If you no longer need your Azure subscription, you can cancel it in the Azure portal.</span></span> <span data-ttu-id="c1fbf-104">Azure サブスクリプションをキャンセルできるのは、アカウント管理者またはサブスクリプションの所有者権限を持つユーザーのみです。</span><span class="sxs-lookup"><span data-stu-id="c1fbf-104">Azure subscriptions can only be canceled by the Account Administrator or by users with Owner rights on the subscription.</span></span>

1. <span data-ttu-id="c1fbf-105">[Azure portal の [サブスクリプション] ページ](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)で、ご利用のサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="c1fbf-105">Select your subscription from the [Subscriptions page in the Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="c1fbf-106">キャンセルするサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="c1fbf-106">Select the subscription that you want to cancel.</span></span>
3. <span data-ttu-id="c1fbf-107">[**概要**] を選び、[**サブスクリプションのキャンセル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c1fbf-107">Select **Overview**, and then select **Cancel subscription**.</span></span>

<span data-ttu-id="c1fbf-108">**サブスクリプションをキャンセルした場合**</span><span class="sxs-lookup"><span data-stu-id="c1fbf-108">**What happens after I cancel my subscription?**</span></span>

<span data-ttu-id="c1fbf-109">キャンセル後、請求は直ちに停止します。</span><span class="sxs-lookup"><span data-stu-id="c1fbf-109">After you cancel, billing is stopped immediately.</span></span> <span data-ttu-id="c1fbf-110">ただし、キャンセルがポータルに表示されるまでに最大 10 分かかります。</span><span class="sxs-lookup"><span data-stu-id="c1fbf-110">However, it can take up to 10 minutes for the cancellation to show in the portal.</span></span> <span data-ttu-id="c1fbf-111">請求期間の途中にキャンセルした場合、期間終了後、通常の請求日に最終請求書が送信されます。</span><span class="sxs-lookup"><span data-stu-id="c1fbf-111">If you cancel in the middle of a billing period, we send the final invoice on your typical invoice date after the period ends.</span></span>

<span data-ttu-id="c1fbf-112">キャンセル後、サービスは無効になります。</span><span class="sxs-lookup"><span data-stu-id="c1fbf-112">After you cancel, your services are disabled.</span></span> <span data-ttu-id="c1fbf-113">つまり、仮想マシンの割り当ては解除され、一時的な IP アドレスは解放され、記憶域は読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="c1fbf-113">That means your virtual machines are de-allocated, temporary IP addresses are freed, and storage is read-only.</span></span>

<span data-ttu-id="c1fbf-114">サブスクリプションのキャンセル後、Microsoft では、お客様がデータにアクセスする必要があったり、気が変わったりした場合に備えて、完全にデータが削除されるまで 30 日から 90 日間の待機期間を設けています。</span><span class="sxs-lookup"><span data-stu-id="c1fbf-114">After your subscription is canceled, Microsoft waits 30 - 90 days before permanently deleting your data in case you need to access it or you change your mind.</span></span> <span data-ttu-id="c1fbf-115">データを保持するために課金されることはありません。</span><span class="sxs-lookup"><span data-stu-id="c1fbf-115">We don't charge you for retaining the data.</span></span> <span data-ttu-id="c1fbf-116">詳細については、「[Microsoft トラスト センターのデータの管理方法](https://go.microsoft.com/fwLink/p/?LinkID=822930&clcid=0x409)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1fbf-116">To learn more, see [Microsoft Trust Center - How we manage your data](https://go.microsoft.com/fwLink/p/?LinkID=822930&clcid=0x409).</span></span>

<span data-ttu-id="c1fbf-117">**Azure サブスクリプションのキャンセル**</span><span class="sxs-lookup"><span data-stu-id="c1fbf-117">**Cancel Azure Subscription**</span></span>

- [<span data-ttu-id="c1fbf-118">サブスクリプションをキャンセルできるユーザー</span><span class="sxs-lookup"><span data-stu-id="c1fbf-118">Who can cancel a subscription?</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support#who-can-cancel-a-subscription)
- [<span data-ttu-id="c1fbf-119">サブスクリプション終了後はどうなりますか</span><span class="sxs-lookup"><span data-stu-id="c1fbf-119">What happens after the subscription</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support#what-happens-after-i-cancel-my-subscription)

<span data-ttu-id="c1fbf-120">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="c1fbf-120">**Recommended Documents**</span></span>

- [<span data-ttu-id="c1fbf-121">サブスクリプションの再アクティブ化</span><span class="sxs-lookup"><span data-stu-id="c1fbf-121">Reactivate subscription</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support#reactivate-subscription)
- [<span data-ttu-id="c1fbf-122">サブスクリプションの切り替え</span><span class="sxs-lookup"><span data-stu-id="c1fbf-122">Switch subscription</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
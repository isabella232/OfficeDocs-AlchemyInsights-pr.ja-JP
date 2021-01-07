---
title: 請求書での支払いに切り替える (小切手/電信送金)
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
- "9004168"
- "7344"
ms.openlocfilehash: de0f727c8c2cdfa830fd9cd600f59a10c33663fd
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755470"
---
# <a name="switch-to-pay-by-invoice-checkwire-transfer"></a><span data-ttu-id="08dfd-102">請求書での支払いに切り替える (小切手/電信送金)</span><span class="sxs-lookup"><span data-stu-id="08dfd-102">Switch to pay by invoice (check/wire transfer)</span></span>

<span data-ttu-id="08dfd-103">お客様の問題の説明に基づいて、解決方法を見つけました。</span><span class="sxs-lookup"><span data-stu-id="08dfd-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="08dfd-104">ほとんどのお客様は、ドキュメントに従って、自分で問題を解決できました。</span><span class="sxs-lookup"><span data-stu-id="08dfd-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="08dfd-105">請求書による支払いに切り替えると、請求書の日付から 30 日以内に請求書を支払うことになります。</span><span class="sxs-lookup"><span data-stu-id="08dfd-105">If you switch to pay by invoice, that means you will pay your bill within 30 days of the invoice date.</span></span> <span data-ttu-id="08dfd-106">請求書で Azure サブスクリプションの支払いを受ける資格を得るには、Azure サポートにリクエストを送信してください。</span><span class="sxs-lookup"><span data-stu-id="08dfd-106">To become eligible to pay for your Azure subscription by invoice, submit a request to Azure support.</span></span> <span data-ttu-id="08dfd-107">リクエストが承認されると、Azure ポータルでサブスクリプションを請求書支払いに切り替えることができます。</span><span class="sxs-lookup"><span data-stu-id="08dfd-107">Once your request is approved, you can switch a subscription to invoice pay in the Azure portal.</span></span>

<span data-ttu-id="08dfd-108">**先に進む前に、請求書支払いオプションのリクエストに関する次の要件および制限を確認してください。**</span><span class="sxs-lookup"><span data-stu-id="08dfd-108">**Before you proceed further, review the following requirements/limitations on requesting invoice payment option:**</span></span>

- <span data-ttu-id="08dfd-109">[Azure ポータル](https://portal.azure.com/)にサインインし、支払い方法に移動して、請求書の支払いが既に事前承認されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="08dfd-109">Sign in to the [Azure portal](https://portal.azure.com/), navigate to payment methods and check if you are already pre-approved for invoice payment.</span></span>
- <span data-ttu-id="08dfd-110">請求書の支払いは、個人アカウントではなく、ビジネス アカウントでのみ利用できます。</span><span class="sxs-lookup"><span data-stu-id="08dfd-110">Invoice pay is only available for business accounts, not for personal accounts.</span></span>
- <span data-ttu-id="08dfd-111">請求書支払いに切り替える前に、すべての未払い料金を支払う必要があります。</span><span class="sxs-lookup"><span data-stu-id="08dfd-111">You must pay all outstanding charges before switching to invoice pay.</span></span>
- <span data-ttu-id="08dfd-112">サポートチームはアカウントを確認して、請求書による支払いの対象かどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="08dfd-112">The support team will review the account to determine if it is eligible for invoice mode of payment.</span></span>
- <span data-ttu-id="08dfd-113">請求書による支払いに切り替えると、クレジット カードまたはデビット カードによる支払いに戻すことはできません。</span><span class="sxs-lookup"><span data-stu-id="08dfd-113">Once you switch to invoice pay, you can't switch back to credit or debit card payment.</span></span>

<span data-ttu-id="08dfd-114">請求書による支払いが承認されたら、 [Azure ポータル](https://portal.azure.com/)で小切手または電信送金を介してAzure サブスクリプションを請求書支払いに切り替えることができます。</span><span class="sxs-lookup"><span data-stu-id="08dfd-114">Once you are approved to pay by invoice, you can switch your Azure subscription to the invoice pay via check or wire transfer in the [Azure portal](https://portal.azure.com/).</span></span>
<span data-ttu-id="08dfd-115">それには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="08dfd-115">To do that:</span></span>

1. <span data-ttu-id="08dfd-116">アカウント管理者として  [Azure ポータル](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="08dfd-116">Sign in to the [Azure portal](https://portal.azure.com/) as the Account Administrator.</span></span> <span data-ttu-id="08dfd-117">" **コストの管理と課金**" を検索して選択します。</span><span class="sxs-lookup"><span data-stu-id="08dfd-117">Search for and select **Cost Management + Billing**.</span></span>
2. <span data-ttu-id="08dfd-118">メニューで、**[請求プロファイル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="08dfd-118">In the menu, choose **Billing profiles**.</span></span>
3. <span data-ttu-id="08dfd-119">請求プロファイルを選択します。</span><span class="sxs-lookup"><span data-stu-id="08dfd-119">Select a billing profile.</span></span>
4. <span data-ttu-id="08dfd-120">*[請求プロファイル]* メニューで、**[支払い方法]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="08dfd-120">In the *Billing profile* menu, select **Payment methods**.</span></span>
5. <span data-ttu-id="08dfd-121">小切手/電信送金で支払う資格があることを示すバナーを選択します。</span><span class="sxs-lookup"><span data-stu-id="08dfd-121">Select the banner that says you are eligible to pay by check/wire transfer.</span></span>

<span data-ttu-id="08dfd-122">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="08dfd-122">**Recommended Documents**</span></span>

- [<span data-ttu-id="08dfd-123">Azure の請求書と使用状況データをリクエスト/ダウンロード/表示する</span><span class="sxs-lookup"><span data-stu-id="08dfd-123">Request/Download/View your Azure billing invoice and usage data</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="08dfd-124">Azure の請求書を受信トレイに直接送信する方法</span><span class="sxs-lookup"><span data-stu-id="08dfd-124">How to email Azure invoices directly to your inbox</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="08dfd-125">請求書での支払い</span><span class="sxs-lookup"><span data-stu-id="08dfd-125">Pay by invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice)
- [<span data-ttu-id="08dfd-126">請求書の内容を理解する</span><span class="sxs-lookup"><span data-stu-id="08dfd-126">Understand terms on your invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-invoice)

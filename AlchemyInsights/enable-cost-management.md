---
title: 原価管理を有効にする
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2020
ms.locfileid: "49680445"
---
# <a name="enable-cost-management"></a><span data-ttu-id="bcd45-102">原価管理を有効にする</span><span class="sxs-lookup"><span data-stu-id="bcd45-102">Enable cost management</span></span>

<span data-ttu-id="bcd45-103">**「組織のコストが無効になっています」の意味は何ですか?**</span><span class="sxs-lookup"><span data-stu-id="bcd45-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="bcd45-104">Enterprise Agreement (EA) または Microsoft Customer Agreement (MCA)のアカウントを使用している組織では、コスト情報と価格の情報へのアクセスを無効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bcd45-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="bcd45-105">Azure ポータルにログインした後は、課金 API を使用して、請求書 (オプトイン後) と使用状況の詳細をプログラムで取得できます。</span><span class="sxs-lookup"><span data-stu-id="bcd45-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="bcd45-106">**その他のユーザーに請求書へのアクセスを許可する方法**</span><span class="sxs-lookup"><span data-stu-id="bcd45-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="bcd45-107">Azure ポータルの **サブスクリプションのブレード** に移動します。</span><span class="sxs-lookup"><span data-stu-id="bcd45-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="bcd45-108">[**請求書**] を選択してから、次に [**請求書にアクセス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="bcd45-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="bcd45-109">アクセスをオンにして、変更を保存すると、サブスクリプション範囲内役割のユーザーは請求書をダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="bcd45-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="bcd45-110">アカウント管理者は、メールで請求書を送信するように設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="bcd45-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="bcd45-111">詳細については、「[メールで請求書を取得する](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date??)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bcd45-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date??).</span></span>

<span data-ttu-id="bcd45-112">**ユーザーを課金リーダーの役割に追加する方法**</span><span class="sxs-lookup"><span data-stu-id="bcd45-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="bcd45-113">Azure ポータルの **サブスクリプションのブレード** に移動します。</span><span class="sxs-lookup"><span data-stu-id="bcd45-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="bcd45-114">[**アクセス制御 (IAM)]** を選択し、[**追加**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="bcd45-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="bcd45-115">[**ロールの選択**] ページで、[**課金リーダー]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="bcd45-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="bcd45-116">招待するユーザーのメールアドレスを入力し、[ **OK**] をクリックして招待状を送信します。</span><span class="sxs-lookup"><span data-stu-id="bcd45-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="bcd45-117">課金内容のリーダーとして招待メールに記載の手順に従ってログインします。</span><span class="sxs-lookup"><span data-stu-id="bcd45-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="bcd45-118">詳細については、「[課金へのアクセス許可を付与](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in) ] を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bcd45-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="bcd45-119">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="bcd45-119">**Recommended documents**</span></span>

- [<span data-ttu-id="bcd45-120">EA ポータルでの DA および AO の表示を有効にする</span><span class="sxs-lookup"><span data-stu-id="bcd45-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="bcd45-121">原価管理に含まれている原価</span><span class="sxs-lookup"><span data-stu-id="bcd45-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="bcd45-122">サポートされる Microsoft Azure の提供</span><span class="sxs-lookup"><span data-stu-id="bcd45-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="bcd45-123">原価分析のコストを確認する</span><span class="sxs-lookup"><span data-stu-id="bcd45-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="bcd45-124">課金情報にアクセス許可を付与する</span><span class="sxs-lookup"><span data-stu-id="bcd45-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="bcd45-125">Microsoft 顧客契約へのアクセス許可の確認</span><span class="sxs-lookup"><span data-stu-id="bcd45-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date??WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)







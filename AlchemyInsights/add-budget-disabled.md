---
title: '[予算を追加] ボタンが無効になっているのはなぜですか?'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822640"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a><span data-ttu-id="1af67-102">[予算を追加] ボタンが無効になっているのはなぜですか?</span><span class="sxs-lookup"><span data-stu-id="1af67-102">Why is the Add budget button disabled for me?</span></span>

<span data-ttu-id="1af67-103">予算を作成するには、次のいずれかの権限が必要です。</span><span class="sxs-lookup"><span data-stu-id="1af67-103">To create a budget, you need one of the following permissions:</span></span>

- <span data-ttu-id="1af67-104">管理グループ、サブスクリプション、リソースグループの範囲</span><span class="sxs-lookup"><span data-stu-id="1af67-104">Management Group, Subscription, Resource Group Scopes</span></span>
- <span data-ttu-id="1af67-105">コスト管理共同作成者</span><span class="sxs-lookup"><span data-stu-id="1af67-105">Cost Management Contributor</span></span>
- <span data-ttu-id="1af67-106">所有者</span><span class="sxs-lookup"><span data-stu-id="1af67-106">Owner</span></span>
- <span data-ttu-id="1af67-107">共同作成者</span><span class="sxs-lookup"><span data-stu-id="1af67-107">Contributor</span></span>
- <span data-ttu-id="1af67-108">エンタープライズ カスタマーのみ: 登録、部門、アカウント スコープ</span><span class="sxs-lookup"><span data-stu-id="1af67-108">Enterprise Customer Only: Enrollment, Department, Account Scopes</span></span>
- <span data-ttu-id="1af67-109">登録管理者 (登録範囲で予算を設定)</span><span class="sxs-lookup"><span data-stu-id="1af67-109">Enrollment Admin (set budget at Enrollment scope)</span></span>
- <span data-ttu-id="1af67-110">部門管理者 (部門範囲で予算を設定)</span><span class="sxs-lookup"><span data-stu-id="1af67-110">Department Admin (set budget at Department scope)</span></span>
- <span data-ttu-id="1af67-111">アカウント所有者 (アカウント範囲で予算を設定)</span><span class="sxs-lookup"><span data-stu-id="1af67-111">Account Owner (set budget at Account scope)</span></span>
- <span data-ttu-id="1af67-112">モダン顧客契約のみ: 請求先アカウント、請求プロファイル、請求書セクションの範囲</span><span class="sxs-lookup"><span data-stu-id="1af67-112">Modern Customer Agreement Only: Billing Account, Billing Profile, Invoice Section Scopes</span></span>
- <span data-ttu-id="1af67-113">Azure サブスクリプション作成者</span><span class="sxs-lookup"><span data-stu-id="1af67-113">Azure subscription creator</span></span>

<span data-ttu-id="1af67-114">**今月の費用がすでに予算超過だったときに予算を作成しました。 アラートを受け取らなかったのはなぜですか?**</span><span class="sxs-lookup"><span data-stu-id="1af67-114">**I created a budget when my cost for the current month was already over-budget. Why did I not receive an alert?**</span></span>  
<span data-ttu-id="1af67-115">予算を作成するときに指定されたコストしきい値をすでに超えている場合、アラートは発生しません。</span><span class="sxs-lookup"><span data-stu-id="1af67-115">If you have already exceeded a given cost threshold when you create a budget that alert will not fire.</span></span> <span data-ttu-id="1af67-116">新しいサイクルが始まると、しきい値に違反するとアラートが発生します。</span><span class="sxs-lookup"><span data-stu-id="1af67-116">Once a new cycle begins, if you breach the threshold then the alert will fire.</span></span>

<span data-ttu-id="1af67-117">**定義された予算アラートしきい値の 1 つを超えた場合、アラートを受信するのはいつですか?**</span><span class="sxs-lookup"><span data-stu-id="1af67-117">**When should I expect to receive an alert after I exceed one of my defined budget alert thresholds?**</span></span>  
<span data-ttu-id="1af67-118">予算は 4 時間ごとに評価されます。</span><span class="sxs-lookup"><span data-stu-id="1af67-118">Budgets are evaluated every 4 hours.</span></span> <span data-ttu-id="1af67-119">使用状況データが予算システムに到達するまでに最低 8 時間かかります。</span><span class="sxs-lookup"><span data-stu-id="1af67-119">It takes a minimum of 8 hours for usage data to reach the budgets system.</span></span> <span data-ttu-id="1af67-120">このため、しきい値を超えてからアラートが発生するまでに 12 時間ほどかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="1af67-120">Given this, alerts may take as long as 12 hours to fire after you exceed a threshold.</span></span>

<span data-ttu-id="1af67-121">**月または請求月のリセット期間を選択すると、[開始日] ボタンが無効になるのはなぜですか?**</span><span class="sxs-lookup"><span data-stu-id="1af67-121">**Why is the Start date button disabled when I select a Month or Billing month reset period?**</span></span>  
<span data-ttu-id="1af67-122">予算は、現在の暦月または現在の請求期間 (請求月が選択されている場合) に合わせて調整されます。</span><span class="sxs-lookup"><span data-stu-id="1af67-122">Budgets are aligned to the current calendar month or current billing period (in the case where Billing Month is selected).</span></span> <span data-ttu-id="1af67-123">したがって、この値を事前に入力します。</span><span class="sxs-lookup"><span data-stu-id="1af67-123">Therefore, we pre-populate this value for you.</span></span>

<span data-ttu-id="1af67-124">**予算作成エクスペリエンスでコストのグラフが表示されないのはなぜですか?**</span><span class="sxs-lookup"><span data-stu-id="1af67-124">**Why do I not see a graph of my costs in the budget creation experience?**</span></span>  
<span data-ttu-id="1af67-125">予算の作成に役立つグラフを表示するには、最低2か月のコストデータが必要です。</span><span class="sxs-lookup"><span data-stu-id="1af67-125">We need a minimum of 2 months of cost data before we can render a graph to assist you with budget creation.</span></span>

<span data-ttu-id="1af67-126">**作成したばかりのサブスクリプションに対して予算を設定できないのはなぜですか?**</span><span class="sxs-lookup"><span data-stu-id="1af67-126">**Why can't I set a budget against a subscription I just created?**</span></span>  
<span data-ttu-id="1af67-127">サブスクリプションを作成した後、データに対して予算を設定する前に、データの処理に 24 〜 48 時間かかります。</span><span class="sxs-lookup"><span data-stu-id="1af67-127">After the creation of a subscription, the data takes 24-48 hours to process before setting a budget against it.</span></span>

<span data-ttu-id="1af67-128">**予算 API リソース**</span><span class="sxs-lookup"><span data-stu-id="1af67-128">**Budget API Resources**</span></span>

- <span data-ttu-id="1af67-129">[予算 API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): 予算を作成および更新するための操作を提供します。</span><span class="sxs-lookup"><span data-stu-id="1af67-129">[Budgets API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to create and update budgets.</span></span> <span data-ttu-id="1af67-130">予算 API を使用すると、予算のしきい値を設定し、そのしきい値に近づくと発生するように複数のアラートを構成できます。</span><span class="sxs-lookup"><span data-stu-id="1af67-130">Using the Budgets API, you can set a budget threshold and configure multiple alerts to fire as you approach that threshold.</span></span> <span data-ttu-id="1af67-131">アラートは、自動化を実行するためにメールまたは Azure アクショングループをトリガーできます。</span><span class="sxs-lookup"><span data-stu-id="1af67-131">Alerts can trigger an email or an Azure Action Group to perform automation.</span></span> <span data-ttu-id="1af67-132">注: この API のフィルタリングは、クエリ API のフィルタリング/ディメンションと一致しません。</span><span class="sxs-lookup"><span data-stu-id="1af67-132">Note: Filtering for this API does not align with Query API filtering / dimensions.</span></span>
- <span data-ttu-id="1af67-133">[予算 API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): v1 よりも優れたコストフィルタリング機能を備えた予算を作成します。</span><span class="sxs-lookup"><span data-stu-id="1af67-133">[Budgets API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Create budgets with greater cost filtering capabilities than v1.</span></span> <span data-ttu-id="1af67-134">フィルター処理は、クエリ API とディメンション API で使用されるコントラクトに合わせて調整されます。</span><span class="sxs-lookup"><span data-stu-id="1af67-134">Filtering aligns to the contract used in our Query and Dimensions APIs.</span></span> <span data-ttu-id="1af67-135">これは、今後使用するために推奨される予算 API です。</span><span class="sxs-lookup"><span data-stu-id="1af67-135">This is the recommended budgets API to use moving forward.</span></span>
- <span data-ttu-id="1af67-136">[ディメンション](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): さまざまなスコープで使用するためにサポートされているディメンションを取得する操作を提供します。</span><span class="sxs-lookup"><span data-stu-id="1af67-136">[Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to get supported dimensions for your usage under a variety of scopes.</span></span> <span data-ttu-id="1af67-137">ディメンション API を使用すると、クエリ API でクエリを生成するための入力として使用できるディメンションのリストを取得できます。</span><span class="sxs-lookup"><span data-stu-id="1af67-137">Using the Dimensions API, you can retrieve a list of dimensions that can be used as inputs for generating queries with the Query API.</span></span>
- <span data-ttu-id="1af67-138">[クエリ](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): 指定したクエリに基づいて、集計されたコストと使用状況のデータを取得する操作を提供します。</span><span class="sxs-lookup"><span data-stu-id="1af67-138">[Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to get aggregated cost and usage data based on the query you supply.</span></span> <span data-ttu-id="1af67-139">Query API を使用すると、使用可能なすべてのディメンション (ディメンション APIからアクセス) で必要なフィルタリング、並べ替え、およびグループ化を指定できます。</span><span class="sxs-lookup"><span data-stu-id="1af67-139">Using the Query API, you can specify your desired filtering, sorting and grouping on all available dimensions (which are accessed from the Dimensions API).</span></span>

<span data-ttu-id="1af67-140">**予測コスト**</span><span class="sxs-lookup"><span data-stu-id="1af67-140">**Forecasted Costs**</span></span>

<span data-ttu-id="1af67-141">**コスト分析にコストの予測が表示されないのはなぜですか?**</span><span class="sxs-lookup"><span data-stu-id="1af67-141">**Why don’t I see forecasts for my costs in Cost Analysis?**</span></span>  
<span data-ttu-id="1af67-142">コスト分析で予測値が表示されない理由は複数ありますが、次のような理由があります。</span><span class="sxs-lookup"><span data-stu-id="1af67-142">There are multiple reasons why the forecast projection might be missing for you in Cost Analysis, some of them are as follows:</span></span>

1. <span data-ttu-id="1af67-143">コストデータが 10 日未満の場合、予測グラフは読み込まれません。</span><span class="sxs-lookup"><span data-stu-id="1af67-143">If your cost data is less than 10 days old, the forecast chart will not load.</span></span> <span data-ttu-id="1af67-144">モデルは、正確な予測のために少なくとも 10 日間の最近のコストデータを必要とします</span><span class="sxs-lookup"><span data-stu-id="1af67-144">The model requires at least 10 days of recent cost data for accurate projections</span></span>
2. <span data-ttu-id="1af67-145">過去の日付を選択した場合、予測グラフは表示されません。</span><span class="sxs-lookup"><span data-stu-id="1af67-145">If you have selected historic dates, then the forecast chart will not be visible.</span></span> <span data-ttu-id="1af67-146">表示する予測グラフの将来の日付を含む日付範囲を選択してください</span><span class="sxs-lookup"><span data-stu-id="1af67-146">Please select a date range with future dates for the forecast chart to be displayed</span></span>
3. <span data-ttu-id="1af67-147">アカウントに複数の通貨がある場合、予測グラフは「すべてのコスト (米ドル)」のコストのみを予測します</span><span class="sxs-lookup"><span data-stu-id="1af67-147">If your account has multiple currencies, the forecast chart will only project costs for 'All costs in USD'</span></span>

<span data-ttu-id="1af67-148">**リソースを変更しても予測が変わらないのはなぜですか?**</span><span class="sxs-lookup"><span data-stu-id="1af67-148">**Why doesn’t the forecast change when I make changes to my resources?**</span></span>  
<span data-ttu-id="1af67-149">予測モデルは、アカウントの変更を説明するのに数日を要し、リソースの変更に基づいた即時の予測は行いません。</span><span class="sxs-lookup"><span data-stu-id="1af67-149">The forecast model requires a couple of days to account for changes in the account and does not make immediate projections based on change in resources</span></span>  
<span data-ttu-id="1af67-150">リソースの増加または減少のより大きなステップの場合、モデルは異常を説明するためにこれらの変更に適応するのに少し時間がかかります</span><span class="sxs-lookup"><span data-stu-id="1af67-150">For larger steps of increase or decrease in resources, the model will take slightly longer to adjust to these changes to account for anomalies</span></span>

<span data-ttu-id="1af67-151">**予約またはマーケットプレイスでの購入後に予測が増加するのはなぜですか?**</span><span class="sxs-lookup"><span data-stu-id="1af67-151">**Why does my forecast increase after I make a reservation or Marketplace purchase?**</span></span>  
<span data-ttu-id="1af67-152">予測モデルは、「実際のコスト」を考慮し、使用量と購入を別々に考慮しません。1 回限りの購入の場合、モデルは、コストの突然の増加を考慮して、10 日後に予測を減らします。</span><span class="sxs-lookup"><span data-stu-id="1af67-152">The forecast model considers your 'Actual Cost' and does not account for usage and purchase separately.For a one-time purchase, the model will decrease the projections after 10 days to account for the sudden increase in costs</span></span>

<span data-ttu-id="1af67-153">**単一のディメンション (たとえば、メートルなど) の予測を確認したい**</span><span class="sxs-lookup"><span data-stu-id="1af67-153">**I want to see forecasts for a single dimension (eg. Meter)**</span></span>  
<span data-ttu-id="1af67-154">予測は現在、個々のメーターではなく、総コストの予測をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="1af67-154">Forecast currently supports total cost projections and not for individual meters.</span></span> <span data-ttu-id="1af67-155">したがって、「グループ化」されたディメンションの場合、予測はディメンション内のすべてのアイテムの合計になります。</span><span class="sxs-lookup"><span data-stu-id="1af67-155">Hence, when 'Grouped by' a dimension, the projections will be for total of all items in the dimension</span></span>

<span data-ttu-id="1af67-156">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="1af67-156">**Recommended Documents**</span></span>

- [<span data-ttu-id="1af67-157">Azure Cost Management の概要</span><span class="sxs-lookup"><span data-stu-id="1af67-157">What is Azure Cost Management?</span></span>](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="1af67-158">Azure Cost Management のベストプラクティス</span><span class="sxs-lookup"><span data-stu-id="1af67-158">Azure Cost Management best practices</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="1af67-159">コストと支出を分析する</span><span class="sxs-lookup"><span data-stu-id="1af67-159">Analyze your costs and spending</span></span>](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="1af67-160">コスト分析を使用して、コストの調査と分析を行う</span><span class="sxs-lookup"><span data-stu-id="1af67-160">Explore and analyze costs with Cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="1af67-161">Azure Cost Management: 価格設定</span><span class="sxs-lookup"><span data-stu-id="1af67-161">Azure Cost Management: Pricing</span></span>](https://azure.microsoft.com/services/cost-management/#pricing)
- [<span data-ttu-id="1af67-162">原価分析のコストを確認する</span><span class="sxs-lookup"><span data-stu-id="1af67-162">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [<span data-ttu-id="1af67-163">ビデオチュートリアル: Azure ポータルで予算を作成する</span><span class="sxs-lookup"><span data-stu-id="1af67-163">Video tutorial: Create a budget in the Azure portal</span></span>](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [<span data-ttu-id="1af67-164">予算を表示およびカスタマイズするための前提条件</span><span class="sxs-lookup"><span data-stu-id="1af67-164">Prerequisites for viewing and customizing budgets</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [<span data-ttu-id="1af67-165">グループの作成と管理</span><span class="sxs-lookup"><span data-stu-id="1af67-165">Create and manage budgets</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [<span data-ttu-id="1af67-166">Azure Action Group および予算 API を使用してオートメーションを構成する</span><span class="sxs-lookup"><span data-stu-id="1af67-166">Configure automation with Azure Action Groups and Budgets API</span></span>](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [<span data-ttu-id="1af67-167">コスト警告を使用して使用と支出を監視する</span><span class="sxs-lookup"><span data-stu-id="1af67-167">Use cost alerts to monitor usage and spending</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="1af67-168">Azure Cost Management のベストプラクティス</span><span class="sxs-lookup"><span data-stu-id="1af67-168">Cost Management best practices</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

<span data-ttu-id="1af67-169">**チュートリアル ビデオ**</span><span class="sxs-lookup"><span data-stu-id="1af67-169">**Tutorial videos**</span></span>

- [<span data-ttu-id="1af67-170">ビデオ チュートリアル: Azure ポータルで予算を作成する</span><span class="sxs-lookup"><span data-stu-id="1af67-170">Create a budget in the Azure portal</span></span>](https://go.microsoft.com/fwlink/?linkid=2146761)
- [<span data-ttu-id="1af67-171">予算 API とアクショングループを使用してコストを管理する</span><span class="sxs-lookup"><span data-stu-id="1af67-171">Manage costs with the Budgets API and Action Groups</span></span>](https://go.microsoft.com/fwlink/?linkid=2147038)
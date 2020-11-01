---
title: '[予算を追加] ボタンが無効になっているのはなぜですか?'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/27/2020
ms.locfileid: "48808193"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>[予算を追加] ボタンが無効になっているのはなぜですか?

予算を作成するには、次のいずれかの権限が必要です。

- 管理グループ、サブスクリプション、リソースグループの範囲
- コスト管理共同作成者
- 所有者
- 共同作成者
- エンタープライズ カスタマーのみ: 登録、部門、アカウント スコープ
- 登録管理者 (登録範囲で予算を設定)
- 部門管理者 (部門範囲で予算を設定)
- アカウント所有者 (アカウント範囲で予算を設定)
- モダン顧客契約のみ: 請求先アカウント、請求プロファイル、請求書セクションの範囲
- Azure サブスクリプション作成者

**今月の費用がすでに予算超過だったときに予算を作成しました。 アラートを受け取らなかったのはなぜですか?**  
予算を作成するときに指定されたコストしきい値をすでに超えている場合、アラートは発生しません。 新しいサイクルが始まると、しきい値に違反するとアラートが発生します。

**定義された予算アラートしきい値の 1 つを超えた場合、アラートを受信するのはいつですか?**  
予算は 4 時間ごとに評価されます。 使用状況データが予算システムに到達するまでに最低 8 時間かかります。 このため、しきい値を超えてからアラートが発生するまでに 12 時間ほどかかる場合があります。

**月または請求月のリセット期間を選択すると、[開始日] ボタンが無効になるのはなぜですか?**  
予算は、現在の暦月または現在の請求期間 (請求月が選択されている場合) に合わせて調整されます。 したがって、この値を事前に入力します。

**予算作成エクスペリエンスでコストのグラフが表示されないのはなぜですか?**  
予算の作成に役立つグラフを表示するには、最低2か月のコストデータが必要です。

**作成したばかりのサブスクリプションに対して予算を設定できないのはなぜですか?**  
サブスクリプションを作成した後、データに対して予算を設定する前に、データの処理に 24 〜 48 時間かかります。

**予算 API リソース**

- [予算 API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): 予算を作成および更新するための操作を提供します。 予算 API を使用すると、予算のしきい値を設定し、そのしきい値に近づくと発生するように複数のアラートを構成できます。 アラートは、自動化を実行するためにメールまたは Azure アクショングループをトリガーできます。 注: この API のフィルタリングは、クエリ API のフィルタリング/ディメンションと一致しません。
- [予算 API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): v1 よりも優れたコストフィルタリング機能を備えた予算を作成します。 フィルター処理は、クエリ API とディメンション API で使用されるコントラクトに合わせて調整されます。 これは、今後使用するために推奨される予算 API です。
- [ディメンション](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): さまざまなスコープで使用するためにサポートされているディメンションを取得する操作を提供します。 ディメンション API を使用すると、クエリ API でクエリを生成するための入力として使用できるディメンションのリストを取得できます。
- [クエリ](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): 指定したクエリに基づいて、集計されたコストと使用状況のデータを取得する操作を提供します。 Query API を使用すると、使用可能なすべてのディメンション (ディメンション APIからアクセス) で必要なフィルタリング、並べ替え、およびグループ化を指定できます。

**予測コスト**

**コスト分析にコストの予測が表示されないのはなぜですか?**  
コスト分析で予測値が表示されない理由は複数ありますが、次のような理由があります。

1. コストデータが 10 日未満の場合、予測グラフは読み込まれません。 モデルは、正確な予測のために少なくとも 10 日間の最近のコストデータを必要とします
2. 過去の日付を選択した場合、予測グラフは表示されません。 表示する予測グラフの将来の日付を含む日付範囲を選択してください
3. アカウントに複数の通貨がある場合、予測グラフは「すべてのコスト (米ドル)」のコストのみを予測します

**リソースを変更しても予測が変わらないのはなぜですか?**  
予測モデルは、アカウントの変更を説明するのに数日を要し、リソースの変更に基づいた即時の予測は行いません。  
リソースの増加または減少のより大きなステップの場合、モデルは異常を説明するためにこれらの変更に適応するのに少し時間がかかります

**予約またはマーケットプレイスでの購入後に予測が増加するのはなぜですか?**  
予測モデルは、「実際のコスト」を考慮し、使用量と購入を別々に考慮しません。1 回限りの購入の場合、モデルは、コストの突然の増加を考慮して、10 日後に予測を減らします。

**単一のディメンション (たとえば、メートルなど) の予測を確認したい**  
予測は現在、個々のメーターではなく、総コストの予測をサポートしています。 したがって、「グループ化」されたディメンションの場合、予測はディメンション内のすべてのアイテムの合計になります。

**おすすめのドキュメント**

- [Azure Cost Management の概要](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management のベストプラクティス](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [コストと支出を分析する](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [コスト分析を使用して、コストの調査と分析を行う](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: 価格設定](https://azure.microsoft.com/services/cost-management/#pricing)
- [原価分析のコストを確認する](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [ビデオチュートリアル: Azure ポータルで予算を作成する](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [予算を表示およびカスタマイズするための前提条件](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [グループの作成と管理](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Azure Action Group および予算 API を使用してオートメーションを構成する](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [コスト警告を使用して使用と支出を監視する](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management のベストプラクティス](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**チュートリアル ビデオ**

- [ビデオ チュートリアル: Azure ポータルで予算を作成する](https://go.microsoft.com/fwlink/?linkid=2146761)
- [予算 API とアクショングループを使用してコストを管理する](https://go.microsoft.com/fwlink/?linkid=2147038)
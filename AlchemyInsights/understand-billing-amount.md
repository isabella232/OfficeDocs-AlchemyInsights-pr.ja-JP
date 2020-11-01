---
title: 請求額について理解する
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
- "9003554"
- "6680"
ms.openlocfilehash: f48ee1e36909515bf81df1ebeb367f91e9a1c9ca
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808496"
---
# <a name="understand-billing-amount"></a>請求額について理解する

**お客様向けの Led (WD):**

- 請求書を確認して理解するには、次を参照してください。 [チュートリアル: 個々の Azure 請求書を確認する](https://docs.microsoft.com/azure/cost-management-billing/understand/review-individual-bill?WT.mc_id=Portal-Microsoft_Azure_Support)
- 請求書の条件を理解する: [Azure の請求書の条件について](https://docs.microsoft.com/azure/cost-management-billing/understand/understand-invoice?WT.mc_id=Portal-Microsoft_Azure_Support)
- Azureの使用料に関する条件を理解する: [使用条件について](https://docs.microsoft.com/azure/cost-management-billing/understand/understand-usage?WT.mc_id=Portal-Microsoft_Azure_Support)
- 請求書のPDFと詳細な毎日の使用状況ファイル (.CSV) のコピーを取得するには: [請求書と使用状況データを取得する](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)

**注** : 請求期間の途中でサブスクリプションまたはリソースをキャンセルしても、前月の使用量に応じた料金が表示される場合があります。 たとえば、請求サイクルが毎月 26 日から翌月の 25 日までで、6 月の請求サイクルの 28 日目である 23 日にサブスクリプションを一時停止した場合、使用した 28 日間の料金が発生する可能性があります。 サブスクリプションをキャンセルしても料金が発生する場合は、料金が発生している他のサポートプランがないか確認してください。 もしあれば、プランをキャンセルしてください。

**Microsoft 顧客契約 (MCA):**

[Microsoft 顧客契約へのアクセス許可の確認方法](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)

- 請求書の内容を確認して理解するには、次を参照してください。[チュートリアル: 個々の Azure 請求書を確認する](https://docs.microsoft.com/azure/cost-management-billing/understand/review-customer-agreement-bill?WT.mc_id=Portal-Microsoft_Azure_Support)
- 請求書の条件を理解する: [Microsoft 顧客契約の請求書のご契約条件について](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-understand-your-invoice?WT.mc_id=Portal-Microsoft_Azure_Support)
- Azure の使用料に関する条件を理解する: [Microsoft 顧客契約の使用条件について](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-understand-your-usage?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Microsoft 顧客契約](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)をお持ちの場合は、[Azure ポータル](https://portal.azure.com/)で使用条件をダウンロードできます。

**Microsoft Partner Agreement (MPA):**

- 請求書の内容を確認して理解するには、次を参照してください。[チュートリアル: Microsoft Partner Agreement を確認する](https://docs.microsoft.com/azure/cost-management-billing/understand/review-partner-agreement-bill?WT.mc_id=Portal-Microsoft_Azure_Support)
- 請求書の条件を理解する: [Microsoft Partner Agreement の請求書のご契約条件について](https://docs.microsoft.com/azure/cost-management-billing/understand/mpa-invoice-terms?WT.mc_id=Portal-Microsoft_Azure_Support)

**Enterprise Agreement (EA)**

- 請求書を確認して理解するには、次の情報を参照してください。[Azure Enterprise Agreement 請求書を理解する](https://docs.microsoft.com/azure/cost-management-billing/understand/review-enterprise-agreement-bill?WT.mc_id=Portal-Microsoft_Azure_Support) 
- Enterprise Agreement (EA customer) を使用している Azure 顧客の場合、組織の請求書はダウンロードできません。 請求書は、登録の請求書を受け取るように設定されているユーザーに送信されます。[Azure portal](https://portal.azure.com/) で使用状況をダウンロードできます。

サービス超過請求書の確認: 

- **エンタープライズ ポータル** にサインインします。 **[レポート]** を選択します
- タブの右上隅で、ビューを **M** から **C** に切り替えて、請求書の期間と一致させます
- 合計 **使用量** は、サービス超過請求書の合計 **拡張** 量と一致する必要があります
- 料金の詳細については、 **[使用量のダウンロード] > [詳細レポートのダウンロード]** に移動してください。 **注** : このレポートには、税金、予約の料金、またはマーケットプレイスの料金は含まれていません。

**Azure Marketplace**

- サードパーティの課金の詳細については、こちらを参照してください。[Azure Marketplace の課金](https://docs.microsoft.com/azure/billing/billing-understand-your-azure-marketplace-charges?WT.mc_id=Portal-Microsoft_Azure_Support)

Marketplace の請求書を確認する:

エンタープライズポータルの [レポート] > [使用状況の概要] でAzure Marketplace の合計をマーケット プレイスの請求書と比較します。 マーケットプレイスの請求書は、Azure Marketplace での購入と使用のみを対象としています。 利用状況の概要の金額には税金は含まれていません。

- **エンタープライズ ポータル** にサインインします。 **[レポート]** を選択します
- タブの右上隅で、ビューを **M** から **C** に切り替えて、請求書の期間と一致させます
- **Azure Marketplace** の合計は、マーケットプレイスの請求書の **合計販売額** と一致する必要があります
- 使用量に基づく料金の詳細については、 **[使用量のダウンロード]** に移動してください。 **[マーケットプレイスの課金]** で、 **[ダウンロード]** を選択します **注** : このレポートには税金が含まれていないか、1 回限りの購入が表示されます

**クラウド ソリューション プロバイダー (CSP)**

- Azure Cloud Solution Provider（Azure CSP）プログラムでの課金の仕組みの詳細: [Azure CSP の課金](https://docs.microsoft.com/azure/cloud-solution-provider/billing/azure-csp-billing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)
- CSP請求書の読み方と理解について学ぶ: [Azure CSP 請求書](https://docs.microsoft.com/azure/cloud-solution-provider/billing/azure-csp-invoice?WT.mc_id=Portal-Microsoft_Azure_Support)

**おすすめのドキュメント**

- 予期しない請求を防ぎ、コストを管理する方法を学ぶ: [予期しない請求を防ぐ](https://docs.microsoft.com/azure/cost-management-billing/manage/getting-started?WT.mc_id=Portal-Microsoft_Azure_Support)
- アカウントの請求アクティビティを監視および管理するための請求またはクレジットアラートの設定: [請求アラートの設定](https://docs.microsoft.com/azure/cost-management-billing/costs/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 支出制限について](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support)
- 外部サービス料金に対する Azure の課金についえ理解する: [外部サービスの請求方法](https://docs.microsoft.com/azure/cost-management-billing/understand/understand-azure-marketplace-charges?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 無料アカウントについてよく寄せられる質問](https://azure.microsoft.com/free/free-account-faq/)
- [Azure の Azure Enterprise Agreement 管理者の役割について理解する](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-ea-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
---
title: 請求書または利用状況のコピーが必要です
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
- "9003801"
- "6804"
ms.openlocfilehash: 5ec935ddd9e273561886831e60c98ae1a542f9da
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808494"
---
# <a name="get-a-copy-of-your-bill-or-usage"></a>請求書または利用状況のコピーを取得する

**Azure 請求書 (.pdf) をダウンロードする**

1. [請求書にアクセスできるユーザー](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)として Azure ポータルの [[サブスクリプション ページ]](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) からサブスクリプションを選択し、 **[請求書]** を選択します
2. PDF請求書のコピーを表示するには、 **[請求書のダウンロード]** をクリックします。 「 **利用できません** 」と表示されている場合は、「[前回の請求期間の請求書が表示されない理由](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)」を参照してください。
3. 請求期間をクリックして、請求書の PDF と詳細な日次利用状況ファイル (.CSV) のコピーを取得することにより、1 日の使用量を表示することもできます。[請求書と使用状況データを取得する](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)

**請求書をメールで取得する (.pdf)**

1. [[サブスクリプション]](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ページから、ご利用のサブスクリプションを選択します。 **[請求書]** に移動して、 **[請求書をメールで送信]** をクリックします
2. **[オプトイン]** をクリックして、利用規約に同意します。 所有しているサブスクリプションごとにオプトインする必要があります。 注: この手順を実行してもメールが届かない場合は、[プロフィールの通信設定](https://account.windowsazure.com/profile)でメールアドレスが正しいことを確認してください
3. [受信トレイに直接メールで送信される Azure の請求書](https://azure.microsoft.com/blog/azure-email-invoices/)

**毎日の使用状況を理解する:** 
[Microsoft Azure の請求書について理解する](https://docs.microsoft.com/azure/cost-management-billing/understand/review-individual-bill?WT.mc_id=Portal-Microsoft_Azure_Support)  

**コスト管理:** [Azure の請求とコスト管理で予期しないコストを防止する](https://docs.microsoft.com/azure/cost-management-billing/manage/getting-started?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Microsoft 顧客契約 (MCA)** :

[Microsoft 顧客契約へのアクセス許可の確認方法](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement) を学ぶ  
[Microsoft 顧客契約](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)をお持ちの場合は、[Azure ポータル](https://portal.azure.com/)で使用状況をダウンロードできます。

**Microsoft 顧客契約の請求書をメールで入手する** :

Microsoft 顧客契約をお持ちの場合は、メールに請求書を送信することができます。 すべての請求プロファイルの所有者、作成者、読者、および請求書管理者は、メールで請求書を受け取ります。 閲覧者は、メールの請求書設定を更新できません

- **コストの管理と課金** を検索します。 **請求プロファイル** を選択します。 [設定] で **[プロパティ]** を選択します。
- [メール請求書]で、 **[メール請求書設定の更新]** を選択します。 [オプトイン] を選びます。 **[更新]** をクリックします。

**エンタープライズ契約 (EA)**

EA の顧客として利用状況データを表示およびダウンロードするには、[料金の表示] ポリシーが有効になっているエンタープライズ管理者、アカウント所有者、または部門管理者である必要があります。

- Azure portal にサインインします。 **コストの管理と課金** を検索します。 請求プロファイルを選択します。
- [利用状況]と料金] を選びます。 ダウンロードする月で、[ダウンロード] を選択します。

**MOSP Azure サブスクリプション**  
[MOSP Azure サブスクリプションの請求書](https://docs.microsoft.com/azure/cost-management-billing/understand/download-azure-invoice?WT.mc_id=Portal-Microsoft_Azure_Support#download-your-mosp-azure-subscription-invoice)

**トラブルシューティング: 前回の請求期間の請求書が表示されない場合**

請求書が表示されない原因として考えられるものを次に示します。

- サブスクリプションの月額料金がクレジット額を超えていないか、無料トライアルを使用中です。 請求書は、支払うべき金額がある場合にのみ生成されます。
- Azure の購読を開始した日から30日経過していません
- 請求書がまだ生成されていません。 請求期間が終了するまでお待ちください
- アカウント管理者でない場合、以前の請求書を利用できない場合があります。 **注** : Microsoftは、Azure CSP のお客様に使用状況レポートや消費データを提供していません。 パートナーセンターの使用状況データはパートナー向け
- AIO (Azure in open) の課金と使用法の詳細: [Azure in open](https://azure.microsoft.com/offers/ms-azr-0111p/)

**おすすめのドキュメント**

- [請求書が表示されない理由](https://docs.microsoft.com/azure/cost-management-billing/understand/download-azure-invoice?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)
- [Azure の請求書と使用状況データをリクエスト/ダウンロード/表示する](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure の請求書を受信トレイに直接送信する方法](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [詳細な使用料金を理解する](https://docs.microsoft.com/azure/cost-management-billing/understand/review-individual-bill?WT.mc_id=Portal-Microsoft_Azure_Support#csv)
- [請求書の内容を理解する](https://docs.microsoft.com/azure/cost-management-billing/understand/understand-invoice?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure CSP の請求書について](https://docs.microsoft.com/partner-center/azure-plan-lp?WT.mc_id=Portal-Microsoft_Azure_Support)

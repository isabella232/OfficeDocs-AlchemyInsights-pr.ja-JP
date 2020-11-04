---
title: 予約インスタンスの購入に対する課金
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
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823249"
---
# <a name="billing-for-reserved-instance-purchase"></a>予約インスタンスの購入に対する課金

予約インスタンス購入は、購入時点で選択したサブスクリプションに紐付いた支払方法で課金されます。 サブスクリプションの種類は、エンタープライズ契約 (オファー番号: MS-AZR-0017P)、従量課金制 (オファー番号: MS-AZR-0003P)、Microsoft 顧客契約、または CSP にする必要があります。

- エンタープライズ サブスクリプションでは、料金が登録した金額コミットメント残高から控除されるか、または過剰として請求されます
- 従量課金制サブスクリプションを利用する場合は、サブスクリプションのクレジットカードまたは請求書による支払い方法で料金が請求されます

**予約のキャンセル**

- **セルフサービス** : [Azure ポータル](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)を使用して、予約済みインスタンスを自分でキャンセルまたは交換できます。 予約を選択し、[返金] または [交換] をクリックします。 交換または返金するには、予約注文の所有者アクセス権が必要です。 予約のみにアクセスしても、返金や交換はできません。 予約注文の所有者に、予約注文へのアクセスを許可するよう依頼してください
- **交換ポリシー:** 予約を同じタイプの別の予約と交換できます。予約交換に **ペナルティはありません** 。 新規予約の合計コミットメントは、交換された予約の払い戻し額と将来の毎月の支払い (該当する場合) の合計よりも大きくする必要があります
- **払い戻しポリシー** : 払い戻しとキャンセルされた将来の支払いの合計は、12 か月のローリングウィンドウで 50,000 米ドルを超えることはできません。 **現在、払い戻しにはペナルティを課していません** が、将来の払い戻しに課す可能性があります

**例外:** セルフサービスの交換およびキャンセル機能は、米国政府のエンタープライズ契約のお客様にはご利用いただけません

- **API / PS / CLI** サポートは、 [Azure予約のキャンセルと払い戻し、セルフサービス交換と払い戻し](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)には利用できません。
- セルフサービスの交換およびキャンセル機能は、米国政府のエンタープライズ契約のお客様にはご利用いただけません。 Pay-As-You-Go や CSP などの他の米国政府のサブスクリプション タイプがサポートされています

詳細については、次の「 [交換と払い戻しのトランザクションの処理方法](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) 」を参照してください。詳細については、次の「[交換と払い戻しのポリシー](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)」を参照してください。その他の質問については、次の「[予約インスタンスの文書を見る](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください

**既存の予約済みインスタンスを交換する (セルフサービス)**

同じタイプの別の予約と交換できます。 予約が不要になった場合は、年間最大 50,000 米ドルまで返金することもできます。 セルフサービスの交換およびキャンセル機能は、米国政府のエンタープライズ契約のお客様にはご利用いただけません。 Pay-As-You-Go や CSP など、他の米国政府のサブスクリプション タイプがサポートされています。 既存の予約を交換または返金するには、予約注文の所有者アクセス権が必要です。

トランザクションを完了する方法については、次の手順を参照してください。

1. [Azure ポータル](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)にサインインします。 返金する予約を選択し、 **[交換]** をクリックします。 2. 購入する VM 製品を選び、数量を入力します。 新規購入の合計金額が返品の合計金額よりも多いことを確認します[購入する前に適切なサイズを決定する](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)。
3. トランザクションを確認して完了します

**予約済みインスタンスの払い戻し**

予約を返金するには、 **[予約の詳細]** に移動し、 **[返金]** をクリックします

**比例配分された払い戻し:**

**払い戻しと交換の比例配分と最小要件の例** 先行予約の例は次の通りです。

- 1 月 1 日に 1 年間の RI を 120 ドルで購入します。
- 4 月 7 日に、この予約の払い戻しまたは交換を希望します
- 予約は 97 日間有効であるため、(1 - 97 ÷ 365) × 120 ドルが返金されます。 (およそ 88.1 ドルです)。 現在、払い戻しに対するペナルティはありません
- 交換する場合、新規購入は 88.1 ドルを超える必要があります
- 現在、払い戻しにペナルティはありません

**請求プランの予約例:**

- 1 月 1 日に 1 年間の RI を月額 10 ドルで購入します。
- 4 月 7 日に、この予約の払い戻しまたは交換を希望します
- 最後に支払いが 7 日間発生したので、(1 - 7 ÷ 31) × 10 ドルが返金されます。 (およそ 7.74 ドルです)。
- キャンセルされる将来の支払いは 80 ドルです。 現在、払い戻しに対するペナルティはありません
- このキャンセルにより、50,000 ドルの払い戻し限度額から 87.74 ドルが差し引かれます。
- 交換する場合、新規購入は 87.74 ドルを超える必要があります

**前回の請求期間の請求書が表示されない場合**

請求書が表示されない原因として考えられるものを次に示します。

- サブスクリプションの月額料金がクレジット額を超えていないか、無料トライアルを使用中です。 請求書は、支払うべき金額がある場合にのみ生成されます。
- Azure の購読を開始した日から30日経過していません
- 請求書がまだ生成されていません。 請求期間が終了するまでお待ちください
- アカウント管理者でない場合、以前の請求書を使用できないことがあります

**Azure ポータル (.pdf) から請求書をダウンロードする**

- [請求書にアクセスできるユーザー](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)として、Azure ポータルの [[サブスクリプション]](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)ページからサブスクリプションを選択します
- **[請求書]** を選択します
- PDF請求書のコピーを表示するには、 **[請求書のダウンロード]** をクリックします。 「 **利用できません** 」と表示されている場合は、「 [前回の請求期間の請求書が表示されない理由](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)」を参照してください。

**請求書をメールで受信します (.pdf)**

- [[サブスクリプション]](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ページから、ご利用のサブスクリプションを選択します。 **[請求書]** をクリックして、請求書をメールで送信します
- **[オプトイン]** をクリックして、利用規約に同意します。 所有しているサブスクリプションごとにオプトインする必要があります

注: この手順を実行してもメールが届かない場合は、[プロフィールの通信設定](https://account.windowsazure.com/profile)でメールアドレスが正しいことを確認してください

**Azure ポータルから使用状況データをダウンロードする**

- [アカウントの管理者](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)として[Azure アカウント センター](https://account.windowsazure.com/Subscriptions)にサインインする
- 請求書と使用状況の情報のサブスクリプションを選択します
- **[請求履歴]** を選択します
- **[現在の明細書を表示する]** を選択して、見積が生成された時点での請求額の見積を表示します
- **[利用状況のダウンロード]** を選択して、日次利用状況データを CSV ファイルとしてダウンロードします。 2 つのバージョンが利用可能であれば、バージョン 2 をダウンロードします

その他の質問: [予約済みインスタンスのドキュメントを見る](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**おすすめのドキュメント**

- [基本的な請求](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [予約済みインスタンス割引を適用する方法を学ぶ](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure の請求書と毎日の使用状況データをダウンロードまたは閲覧する](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [予約済みインスタンス割引を適用する方法を学ぶ](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [従量課金制サブスクリプションの予約済みインスタンスの使用状況を理解する](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [エンタープライズ加入契約の予約済みインスタンスの使用状況を理解する](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [予約済みインスタンスを含まない Windows ソフトウェア コスト](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [パートナー セントラル クラウド ソリューション プロバイダー (CSP) プログラムの予約済みインスタンス](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)
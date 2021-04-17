---
title: 予約のキャンセル
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
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819697"
---
# <a name="cancelling-reservation"></a>予約のキャンセル

- **セルフサービス**: [Azure ポータル](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)を使用して、予約済みインスタンスを自分でキャンセルまたは交換できます。 予約を選択し、[返金] または [交換] をクリックします。 交換または返金するには、予約注文の所有者アクセス権が必要です。 予約のみにアクセスしても、返金や交換はできません。 予約注文の所有者に、予約注文へのアクセスを許可するよう依頼してください
- **交換ポリシー:** 予約を同じタイプの別の予約と交換できます。予約交換に **ペナルティはありません**。 新規予約の合計コミットメントは、交換された予約の払い戻し額と将来の毎月の支払い (該当する場合) の合計よりも大きくする必要があります
- **払い戻しポリシー**: 払い戻しとキャンセルされた将来の支払いの合計は、12 か月のローリングウィンドウで 50,000 米ドルを超えることはできません。 **現在、払い戻しにはペナルティを課していません** が、将来の払い戻しに課す可能性があります  
    **例外:** セルフサービスの交換およびキャンセル機能は、米国政府のエンタープライズ契約のお客様にはご利用いただけません
- **API / PS / CLI** サポートは、[Azure予約のキャンセルと払い戻し、セルフサービス交換と払い戻し](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)には利用できません。
- セルフサービスの交換およびキャンセル機能は、米国政府のエンタープライズ契約のお客様にはご利用いただけません。 Pay-As-You-Go や CSP などの他の米国政府のサブスクリプション タイプがサポートされています

詳細情報: [返品および交換トランザクションの処理方法](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
詳細情報: [交換および返金ポリシー](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
その他の質問: [予約済みインスタンスのドキュメントにアクセスする](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**既存の予約済みインスタンスを交換する (セルフサービス)**

同じタイプの別の予約と交換できます。 予約が不要になった場合は、年間最大 50,000 米ドルまで返金することもできます。 セルフサービスの交換およびキャンセル機能は、米国政府のエンタープライズ契約のお客様にはご利用いただけません。 Pay-As-You-Go や CSP など、他の米国政府のサブスクリプション タイプがサポートされています。 既存の予約を交換または返金するには、予約注文の所有者アクセス権が必要です。

トランザクションを完了する方法については、次の手順を参照してください。

1. [Azure ポータル](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)にサインインします。 返金する予約を選択し、**[交換]** をクリックします
2. 購入する VM 製品を選び、数量を入力します。 新規購入の合計が返品の合計よりも多いことを確認し、[購入する前に適切なサイズを決定](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)します
3. トランザクションを確認して完了します

**予約済みインスタンスの払い戻し**

予約を返金するには、**[予約の詳細]** に移動し、**[返金]** をクリックします

**比例配分された払い戻し:**

**払い戻しと交換の比例配分と最小要件の例**  
事前予約の例:

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

**おすすめのドキュメント**

- [返品および交換トランザクションの処理方法](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [交換および返金ポリシー](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)
---
title: サブスクリプションやアカウントの無効化ルール
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
- "9003559"
- "6676"
ms.openlocfilehash: 6a350c6bca18306e64f647cfa3a7f14fa204109b
ms.sourcegitcommit: 9626d39e5891f83774ba31574a00b0bae92ad442
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/24/2020
ms.locfileid: "48758621"
---
# <a name="azure-subscription-disabled"></a>Azure サブスクリプションの無効化

お使いのクレジットの有効期限が切れている、支出制限に達した、請求が期限切れになった、クレジット カードの限度額に達した、またはアカウント管理者にサブスクリプションをキャンセルされたなどの理由により、Azure サブスクリプションが無効になっている可能性があります。 サブスクリプションを再び有効にする方法については、以下を参照してください。 詳細情報: [Azure サブスクリプションを再度有効にする](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable?WT.mc_id=Portal-Microsoft_Azure_Support)

**Azure サブスクリプションをもう一度有効にします (サブスクリプションが偶発的にキャンセルされた場合)**。[アカウント管理者](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) は、アカウント センターでキャンセルされた従量課金制のサブスクリプションを再アクティブ化できます。

1. [アカウント センター](https://account.windowsazure.com/Subscriptions)にサインインします。
2. キャンセルされたサブスクリプションを選択します。 **再アクティブ化** をクリックします。

その他の種類のサブスクリプションについては、[サポート サービス](https://portal.azure.com/?#blade/Microsoft_Azure_Support/HelpAndSupportBlade)にお問い合わせの上、サブスクリプションを再アクティブ化します。

**有効期限切れのクレジット カード**

**Azure 無料アカウント** にサインアップすると、無料試用版サブスクリプションを取得できます。ここでは、30 日間有効な 200 USD の Azure クレジットと 12 か月間の無料サービスが提供されます。 30 日が経過すると、Azure はサブスクリプションを無効化します。 お客様のサブスクリプションが無効化されるのは、お使いのサブスクリプションを含むクレジットと無料サービスの使用量以外に誤って利用料金が発生することを防ぐためです。 Azure サービスを継続して使用するには、[サブスクリプションのアップグレード](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)を行う必要があります。 アップグレード後も、お使いのサブスクリプションで引き続き 12 か月間の無料サービスを利用できます。 無料サービスと使用量以外の使用状況についてのみ課金されます。  
詳細情報: [有効期限切れのクレジット カード](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable?WT.mc_id=Portal-Microsoft_Azure_Support#your-credit-is-expired)

**支出制限に達しました**

使用量が支出制限に達すると、Azure はその課金期間の残りの期間のサブスクリプションを無効にします。 お客様のサブスクリプションが無効化されるのは、お使いのサブスクリプションを含むクレジットの使用量以外に誤って利用料金が発生することを防ぐためです。 支出制限を削除するには、「[Azure の支出制限](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。  
詳細情報: [支出制限に達した場合](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled?WT.mc_id=Portal-Microsoft_Azure_Support#you-reached-your-spending-limit)

**請求書の期限切れ**

過去に期限の切れた残高を解決するには、「[Azure からのメール取得後に過去の Azure サブスクリプションの期限切れ残高を解決する](https://docs.microsoft.com/azure/billing/billing-azure-subscription-past-due-balance?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。

**請求額がクレジット カードの上限を超えています**

この問題を解決するには、[別のクレジット カードに切り替えます](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support)。 または、ビジネスで使用する場合は、[請求書による支払いに切り替える](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice?WT.mc_id=Portal-Microsoft_Azure_Support)ことができます。

**注**: 再び有効になったサブスクリプションには、新しいサブスクリプション記念日 (SA) が割り当てられます。 サブスクリプションを中断した日数 (間隔) は、元のサブスクリプション記念日に追加されます。 記念日が29日、30日、または31日の場合、SA の日付は次の月の最初の日付に設定されます。  
例: 

- 元のサブスクリプション記念日が 25 日の場合は、以下のようになります。
- サブスクリプションが 10 月 3 日に中断され、10 月 9 日に再び有効になりました。
- サブスクリプションは 6 日間無効でした (間隔は 6)。
- その間隔が元のサブスクリプション記念日に追加され、その合計 (25 + 6 = 31) が新しいサブスクリプション記念日になります。 

**注**: この例では、SA の日付が 28 を超えているため、新しい SA の日付が次の月の最初の日付になります。

**おすすめのドキュメント**

- [サブスクリプションの切り替え](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)  
- [サブスクリプションのキャンセル](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)  
- [Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace/?source=datamarket)
- [アカウント管理者](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)を検索
- [Azure サブスクリプションが無効になった場合の対処方法](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 支出制限](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support)

---
title: Azure の請求の所有権を譲渡する
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
- "9003560"
- "6849"
ms.openlocfilehash: 454ce626862bb4a2361abccd92ad0099b534388c
ms.sourcegitcommit: 059ad2936788266ea9714ec8c66d407d7261aeb6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/29/2020
ms.locfileid: "49736883"
---
# <a name="transfer-azure-billing-ownership"></a>Azure の請求の所有権を譲渡する

譲渡するサブスクリプションを所有する課金アカウントの管理者として [Azure portal](https://portal.azure.com/)にサインインします。 自分が管理者かどうかわからない場合、または管理者を特定する必要がある場合は、「[アカウントの課金管理者を特定する](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)」を参照してください。

1. _コストの管理と請求_ で検索します。
1. 左側のウィンドウから **[サブスクリプション]** を選択します。 アクセス権によっては、課金スコープを選択してから **[サブスクリプション]** または **[Azure サブスクリプション]** を選択する必要がある場合があります。
1. 譲渡するサブスクリプションの **[課金所有権の譲渡]** を選択します。
1. サブスクリプションの新しい所有者となるアカウントの課金管理者であるユーザーのメール アドレスを入力し、**[譲渡要求の送信]** を選択します。
1. ユーザーには、譲渡要求を確認するための手順が記載されたメールが届きます。 譲渡要求を承認するには、ユーザーはメール内のリンクを選択し、指示に従います。

サブスクリプションの課金所有権を別の Azure AD テナントのユーザーのアカウントに譲渡すると、サブスクリプション内のリソースを管理するためのすべての[ロールベースのアクセス制御 (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) の割り当てが完全に削除されます。 新しい所有者のみが、サブスクリプション内のリソースを管理するためのアクセス権を持ちます。 詳細については、「[サブスクリプションを別の Azure AD テナント内のユーザーに譲渡する](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。

_**請求書への重要な影響**_: Azure サブスクリプションの課金所有権を譲渡した場合、料金は日割り計算されます。 次の方法で請求書にアクセスできます。  

1.  [請求書へのアクセス権を持つユーザー](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)として Azure portal の [[サブスクリプション] ページ](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) からサブスクリプションを選択し、 **[請求書]** を選択します。
1. PDF 請求書のコピーを表示するには、 **[請求書のダウンロード]** をクリックします。 " _利用できません_" と表示されている場合は、「 [前回の請求期間の請求書が表示されない理由](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)」を参照してください。
1. また、**請求期間** をクリックし、請求書の PDF と詳細な日次使用量ファイル (.CSV) のコピーを取得して、日ごとの使用量を表示することもできます。 詳細については、「 [請求書と使用状況データを取得する](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。

**お勧めのドキュメント**

- [Azure サブスクリプションの請求所有権を別のアカウントに譲渡する](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Azure サブスクリプションの請求所有権の譲渡について](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Visual Studio、Microsoft Partner Network (MPN)、Pay as you go 開発/テスト サブスクリプションの譲渡](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [所有権の譲渡についての FAQ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [所有権の移転に関する問題のトラブルシューティング](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)

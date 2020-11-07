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
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922250"
---
# <a name="transfer-azure-billing-ownership"></a>Azure の請求の所有権を譲渡する

譲渡するサブスクリプションを所有している請求アカウントの管理者として [Azure ポータル](https://portal.azure.com/)にサインインします。 自分が管理者なのかどうかがわからない場合、または管理者を決定する必要がある場合には、「[Determine account billing administrator (アカウントの課金管理者を決定する)](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)」を参照してください。

- **コスト管理 + 請求** で検索します。
- 左側のウィンドウから **[サブスクリプション]** を選択します。 アクセスに応じて、課金範囲を選択してから **[サブスクリプション]** または **[Azure サブスクリプション]** を選択する必要がある場合があります。
- 譲渡するサブスクリプションの **[請求の所有権を譲渡する]** を選択します
- サブスクリプションの新しい所有者となるアカウントの請求管理者であるユーザーのメールアドレスを入力し、 **[転送リクエストの送信]** を選択します
- ユーザーには、転送リクエストを確認するための手順が記載されたメールが届きます。 転送要求を承認するには、ユーザーはメール内のリンクを選択し、指示に従います。

**注** : サブスクリプションの請求所有権を別の Azure AD テナントのユーザーのアカウントに譲渡すると、サブスクリプション内のリソースを管理するためのすべての[役割ベースのアクセス制御 (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) の割り当てが完全に削除されます。 新しい所有者のみが、サブスクリプション内のリソースを管理するためのアクセス権を持ちます。 詳細については、「[別のAzureADテナントのユーザーへのサブスクリプションの転送](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。

**おすすめのドキュメント**

- [Azure サブスクリプションの請求所有権を別のアカウントに譲渡する](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Azure サブスクリプションの請求所有権の譲渡について](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Visual Studio、Microsoft Partner Network (MPN)、Pay as you go 開発/テスト サブスクリプションの譲渡](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [所有権の譲渡についての FAQ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [所有権の移転に関する問題のトラブルシューティング](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)

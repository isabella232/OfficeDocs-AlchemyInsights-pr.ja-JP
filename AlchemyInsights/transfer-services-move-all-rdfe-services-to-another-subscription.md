---
title: サービスの転送 - すべての RDFE サービスを別のサブスクリプションに移動する
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
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940066"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>サービスの転送 - すべての RDFE サービスを別のサブスクリプションに移動する

**リソースを移動する**

Azure portal、Azure PowerShell、Azure CLI、または REST API を使用してリソースを移動すると、Azure リソースを同じサブスクリプションの中の別の Azure サブスクリプションまたはリソース グループに移動できます。

リソースを移動する前に、以下を参照してください。

- [リソースの移動前のチェック リスト](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [移動可能なサービス](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [移動の検証方法](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [サービスの移動ガイダンス](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

既存のリソースを別のリソース グループまたはサブスクリプションに移動するには、次を使用できます。

- [Azure portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

チュートリアル: [既存のリソースを別のリソース グループまたはサブスクリプションに移動する](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Azure Resource Manager でエラーをトラブルシューティングする**

以下の記事を参照して、いくつかの一般的な Azure 展開エラーについて学習し、それらを解決するための情報を受け取ります。 展開エラーのエラー コードが見つからない場合は、[エラーコードの検索](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)を参照してください。

- [展開エラーのトラブルシューティング](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [既存のリソースを新しいリソース グループまたはサブスクリプションに移動する際のトラブルシューティング](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

無料から従量課金制への切り替えなど、Azure サブスクリプションをアップグレードする場合は、サブスクリプションを変換する必要があることに注意してください。

- 無料試用版をアップグレードするには、「[無料試用版のアップグレードまたは Microsoft Imagine Azure サブスクリプションを従量課金制にアップグレードする](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)」を参照してください。
- 従量課金制のアカウントを変更するには、「[Azure従量課金制のサブスクリプションを別のオファーに変更する](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)」を参照してください。

**Azure サブスクリプションを Azure Active Directoryテ ナントに追加または関連付けするには、以下の操作を行います。**

1. サインインして、[Azure portal の [サブスクリプション] ページ](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)から使用するサブスクリプションを選択します。
2. **[ディレクトリの変更]** を選択します。
3. 表示される警告を確認してから、**[変更]** を選択します。
4. サブスクリプションのディレクトリが変更され、成功メッセージが表示されます。
5. *ディレクトリ* スイッチャーを使用して、新しいディレクトリに移動します。 すべてが正しく表示されるまでに最大 10 分かかる場合があります。

**おすすめのドキュメント**

- [Azure サブスクリプションの請求所有権の譲渡について](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [既存のリソースを新しいリソース グループまたはサブスクリプションに移動する](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Azure portal を使用してリソースを管理する](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)

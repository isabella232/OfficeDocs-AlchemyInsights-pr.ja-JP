---
title: サポートされているサブスクリプションの種類
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
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072165"
---
# <a name="supported-subscription-types"></a>サポートされているサブスクリプションの種類

詳細については、サポートされているサブスクリプションの種類を確認してください。

[サポートされているサブスクリプションの種類](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**請求の所有権を譲渡する**

転送するサブスクリプションを持つ請求先アカウントの[アカウント管理者](https://ms.portal.azure.com/)としての Azure ポータル

- **コスト管理 + 請求** で検索します。 左側のウィンドウから **[サブスクリプション]** を選択します。 アクセスに応じて、課金範囲を選択してから、**[サブスクリプション]** または **[Azure サブスクリプション]** を選択する必要がある場合があります。
- 転送するサブスクリプションの [請求所有権の転送] を選択します
- サブスクリプションの新しい所有者となるアカウントの請求管理者であるユーザーのメールアドレスを入力し、**[転送リクエストの送信]** を選択します
- ユーザーには、譲渡要求を確認するための手順が記載されたメールが届きます。 譲渡要求を承認するには、ユーザーはメール内のリンクを選択し、指示に従います。

注: サブスクリプションの請求所有権を別の Azure AD テナントのユーザーのアカウントに譲渡すると、サブスクリプション内のリソースを管理するためのすべての[役割ベースのアクセス制御 (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) 割り当てが完全に削除されます。 新しい所有者のみが、サブスクリプション内のリソースを管理するためのアクセス権を持ちます。 詳細については、「[別のAzureADテナントのユーザーへのサブスクリプションの転送](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。

**サブスクリプションの所有権を譲渡する**

サブスクリプション内のリソースを管理するためのサブスクリプション所有権転送の前提条件ロールベースアクセス (RBAC) は、アクセスを失います。 テナントへの既存のサブスクリプションの追加の詳細については、「[Azure ActiveDirectory への Azure サブスクリプションの関連付けまたは追加](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。

- 現在の請求サイクルからの既存の未払い金額のサブスクリプション転送は、新しいアカウントの新しい支払い手段に転送されません。 新しいアカウントでユーザーが利用できる情報は、サブスクリプションの先月の費用のみになります。 それ以外の使用履歴と請求履歴は、サブスクリプションと一緒に転送されません。
- Enterprise Agreement (EA) サブスクリプションの請求所有権の譲渡は、現在Enterprise Agreement Portalでのみサポートされています。
- Visual Studio、BizSpark、Microsoft パートナーネットワークなどのクレジット指向のサブスクリプションを新しいユーザーに転送するには、転送要求を受け入れるために Visual Studio / Microsoft パートナーネットワークライセンスが必要です。
- 仮想マシン、ディスク、Web サイトなどのすべてのリソースは、新しいアカウントに正常に転送されます。 テナント間のサブスクリプション転送では、次のリソースが影響を受ける可能性があります。

**Azure AD Domain Services**

Azure Key Vault

- 特に顧客が AzureActive Directory 関連の認証を使用している場合、[SQL 関連のユーザーとデータベース](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support)が影響を受ける可能性があります
- Azure Active Directory 認証で構成された **App Services** が影響を受ける可能性があります
- Azure サブスクリプションに接続されている **Visual Studio Team** Services アカウントは、接続されている Azure サブスクリプションがキャンセルされると一時的にアクセスできなくなる場合があります

**おすすめのドキュメント**

請求の所有権を承諾した後の手順:

- 請求の所有権を保持し、サブスクリプションのタイプを変更するには、次を参照してください: [Azureサブスクリプションを別のプランに切り替える](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Visual Studio、Microsoft Partner Network (MPN)、および Pay as you go Dev / Test サブスクリプションの移行](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Enterprise Agreement (EA) サブスクリプションの請求所有権の移転](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [所有権の譲渡についての FAQ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [所有権の移転に関する問題のトラブルシューティング](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
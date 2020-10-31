---
title: サブスクリプションへのアクセス
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/27/2020
ms.locfileid: "48808197"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>ブラウザーの問題が原因で、Azure にサインインできない (ブラウザーがハングする、処理中のままである、読み込みできないなど)

停止の影響を受ける可能性があります。 「[Azure 正常性状態](https://status.azure.com/status/history/)」で、継続的に停止していないか確認してください。

すべてのアクティブな Azure セッションからログアウトしてください。 Web ブラウザーのプライベート モードまたはシークレット モードを開始します。

また、上記の操作でも機能しない場合は、ブラウザーの更新、別のブラウザーの使用、キャッシュ Cookie の削除などを試すこともできます。

詳細については、「[サインインの問題に関するトラブルシューティング](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)」を参照してください。

**サブスクリプションにアクセスできない**

[[Azure portal](https://portal.azure.com/)] で、右上のアカウントから正しい Azure ディレクトリが選択されていることを確認します。

[[Azure アカウント センター](https://account.windowsazure.com/Subscriptions)] で、アカウントを使用しているのがアカウント管理者であることを確認します。

詳細については、「[サブスクリプションが見つからない場合のトラブルシューティング](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。

**請求履歴にアクセスできない**

アカウント管理者は、「[新しいユーザーを追加または削除](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)」で、請求情報にアクセスするユーザーが Azure Active Directory にゲスト ユーザーとして追加されたことを確認する必要があります。

ユーザーは、「[ユーザーにロールを割り当てる](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)」でグローバル管理者ロールが割り当てられている必要があります。

これを投稿し、「[請求へのアクセスを許可](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)」で RBAC ポリシーを使用してユーザーに請求へのアクセス許可を割り当てることができます。

**おすすめのドキュメント**

-   [Azure サブスクリプションの管理にサインインできない](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)
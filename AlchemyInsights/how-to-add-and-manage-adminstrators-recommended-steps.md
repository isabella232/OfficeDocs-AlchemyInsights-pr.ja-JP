---
title: 管理者の追加および管理方法 - 推奨される手順
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963792"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>管理者の追加および管理方法 - 推奨される手順

お客様の問題の説明に基づいて、解決方法を見つけました。 ほとんどのお客様は、ドキュメントに従って、自分で問題を解決できました。

**サブスクリプション管理者または共同管理者を編集する**

- アカウント管理者は両方の役割を編集できますが、サブスクリプション管理者は [Azure ポータル](https://ms.portal.azure.com/#home)でのみ共同管理者を変更できます。
- [Azure サブスクリプション管理者を追加または変更する](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**サブスクリプション管理者または内部の共同管理者 (AIRS) を更新する**

サービス管理者または共同管理者は、次の手順を使用して、この操作をセルフサービスで実行できます。

1. [Azure ポータル](https://ms.portal.azure.com/#home)にログインし、左側のブレードの **[コスト管理と請求**] をクリックします。
2. サブスクリプションのある品目をクリックします。 サブスクリプションの概要が開きます。
3. **[サブスクリプション]** ブレードで、**[プロパティ]** をクリックします。 
4. **[サービス管理者**] ボタンをクリックします。
5. サービス管理者として設定するユーザーのメールを入力し、**[OK]** をクリックします。

**共同管理者の追加/変更/削除**

1. サービス管理者として [Azure ポータル](https://ms.portal.azure.com/#home)にログインします。
2. [[サブスクリプション]](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) を開き、サブスクリプションを選択します。 (共同管理者は、サブスクリプション範囲でのみ割り当てることができます。)
3. **[アクセス制御 (IAM)]** > **[従来の管理者]** > **[追加]** > **[共同管理者の追加]** の順に移動し、**[共同管理者を追加]** ウィンドウを開きます ([共同管理者の追加] オプションが無効になっている場合は、権限がないことを示します)。
4. 追加するユーザーを選択し、**[追加]** をクリックします。

**詳細情報:**
- [共同管理者を追加する](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [共同管理者を削除する](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [サービス管理者を変更する](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [アカウント管理者を表示する](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [RBAC および Azure ポータルを使用してアクセスを管理する](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Azure Active Directory を使用してユーザーを追加/削除する**

Azure Active Directory (Azure AD) 組織から、新しいユーザーを追加したり、既存のユーザーを削除したりできます。

1. 新しいユーザーを追加するには、組織のユーザー管理者として [Azure ポータル](https://ms.portal.azure.com/#home)にログインします。
2. **[Azure Active Directory]** を選択し、**[ユーザー]** を選択してから、**[新しいユーザー]** をクリックします。
3. **[ユーザー]** ページで、必要な情報を入力します。 **[作成]** をクリックします。 ユーザーが作成され、Azure AD テナントに追加されます。

**詳細情報**:

- [新しいユーザーを追加する](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [ユーザーを削除する](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Azure Active Directory を使用してユーザーのプロファイル情報を追加または更新する](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**おすすめのドキュメント**

- [役割ベースのアクセス制御 (RBAC) とは](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Azure のさまざまな役割を理解する](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Azure Active Directory での管理者役割のアクセス許可](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [チュートリアル: RBAC および Azure ポータルを使用してユーザーにアクセス権を付与する](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Azure での RBAC のトラブルシューティング](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Azure 管理グループでリソースを編成する](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [メールで Azure 請求書のコピーを要求する方法](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Azure でクレジット カードまたはデビット カードを追加、更新、または削除する方法](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [サブスクリプションの管理 (再アクティブ化/キャンセル/切り替え)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)




---
title: MCA に関連付けられている販売先住所および請求先住所の更新 - 推奨される手順
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004166"
- "7325"
ms.openlocfilehash: 5c0f4e7e92081a60be1f6930100ed08ce91ad545
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320035"
---
# <a name="update-sold-to-and-bill-to-address-associated-to-your-mca---recommended-steps"></a>MCA に関連付けられている販売先住所および請求先住所の更新 - 推奨される手順

Microsoft 顧客契約 (MCA) に関連付けられている販売先住所および請求先住所を更新できます。 

**注**: Azure Active Directory のユーザー プロファイル情報を変更できるのは、ユーザー管理者だけです。 ユーザーの管理者役割が割り当てられていない場合は、ユーザー管理者に問い合わせてください。 ユーザーのプロファイルの変更の詳細については、「[Azure Active Directory を使用してユーザーのプロファイル情報を追加または更新する](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)」を参照してください。

**販売先住所**: 販売先住所は、課金アカウントの責任者である組織または個人の住所および連絡先情報です。 課金アカウント用に作成されたすべての請求書に表示されます。

**請求先住所**: 請求先住所は、課金アカウントに対して生成された請求書の責任者である組織または個人の住所および連絡先情報です。 MCA の課金アカウントの場合、課金プロファイルごとに請求先住所があり、請求プロファイル用に作成された請求書に表示されます。

**MCA の課金アカウントの販売先住所を更新するには**:

1. MCA の課金アカウントに対して所有者または投稿者ロールを持つメール アドレスを使用して、Azure ポータルにサインインします。
1. **[コストの管理** + **課金]** を検索します。
1. **[プロパティ]** > **[販売先住所の更新]** の順にクリックします。
1. 新しい住所を入力し、**[保存]** をクリックします。

一部のアカウントでは、販売先住所を更新する前に追加の確認が必要です。 アカウントに手動承認が必要な場合は、Azure サポートに連絡するように求められます。

**MCA の課金アカウントの住所** を更新するには: 

1. MCA の課金アカウントまたは MCA の課金プロファイルに対して所有者または投稿者ロールを持つメール アドレスを使用して、Azure ポータルにサインインします。
1. **[コストの管理** + **課金]** を検索します。
1. **[課金プロファイル]** をクリックし、課金プロファイルを選択して課金住所を更新します。
1. **[プロパティ]** > **[住所の更新]** の順にクリックします。
1. 新しい住所を入力し、**[保存]** を選択します。

**おすすめのドキュメント**

[Azure 課金アカウントの連絡先情報を変更する](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile)   
[課金アカウントの設定を更新する](https://docs.microsoft.com/microsoft-store/update-microsoft-store-for-business-account-settings)  
[Azure での Microsoft 顧客契約の管理者の役割を理解する](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
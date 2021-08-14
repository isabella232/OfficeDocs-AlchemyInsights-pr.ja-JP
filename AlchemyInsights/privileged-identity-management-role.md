---
title: 特権 ID 管理のロール
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
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973234"
---
# <a name="privileged-identity-managementpim-role"></a>特権 ID 管理 (PIM) のロール

**ロールのアクティブ化を行った後、権限が付与されない**

Azure AD Privileged Identity Management（PIM）でロールをアクティブ化すると、そのアクティブ化が、特権ロールを必要とするすべてのポータルに即座に伝達されない場合があります。 場合によっては、変更が伝播されたとしても、ポータルで Web キャッシュを行うと、変更がすぐに有効にならないことがあります。

アクティブ化が遅れる場合は、次の手順に従ってください。

1. Azure ポータルからサインアウトしてから、再度サインインします。 Azure AD ロールまたは Azure リソース ロールをアクティブ化すると、アクティブ化のステージが表示されます。 すべての段階が完了すると、「サインアウト」リンクが表示されます。 このリンクを使用してサインアウトできます。 これにより、アクティブ化遅延のほとんどの場合が解決されます。
2. PIMで、自分がロールのメンバーとしてリストされていることを確認します。
3. Exchange 管理者ロールをアクティブ化する場合は、必ずサインアウトしてから再度サインインしてください。 問題が解決しない場合は、サポート チケットを開き、問題として提起します。 Exchange 管理者ロールを使用してセキュリティ/コンプライアンス センターにアクセスしている場合は、次の手順を参照してください。
4. セキュリティ/コンプライアンス センターにアクセスするためにロールをアクティブ化する場合、または SharePoint 管理者のロールをアクティブ化する場合、数分から数時間までのアクティブ化の遅延が発生します。 これは既知の問題であり、これらのチームと積極的に協力して、この問題をできるだけ早く解決できるよう取り組んでいます。

詳しくは、以下を参照してください。

- [PIM で Azure AD ロールをアクティブ化する](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [PIM で Azure リソース ロールをアクティブ化する](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**ロールを非アクティブ化した後、またはロールのアクティブ化の有効期限が切れた後、アクセス許可が削除されない**

Azure AD Privileged Identity Management でロールを非アクティブ化する場合、またはロールのアクティブ化期間が終了すると、引き続きアクセスできるようになるまでに遅延が発生する場合があります。

非アクティブ化が遅れる場合は、次の手順に従ってください。

1. Exchange管理者ロールを非アクティブ化する場合、またはロールのアクティブ化期間が満了していて、権限が削除されるまでに大幅な遅延が発生していることに気づいた場合は、サポート チケットを開き、サポート エンジニアに、この問題について Office 内の特権アクセス管理 (PAM) チームにチケットを提出するのを手伝ってもらうように伝えます。
2. アクティベーション期間が終了してもブラウザー セッションが開いている場合は、ブラウザーを閉じてください。 そのセッションを閉じるまで、ロールを引き続き使用できます。 これは既知の問題であり、アクティベーションの有効期限が切れたときに、各セッションをアクティブに取り消すための修正の可能性を検討しています。

この2つのシナリオとは異なる遅延がある場合は、サポート チケットを開いてください。

---
title: 'RBAC ロール '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923136"
---
# <a name="rbac-rules"></a>RBAC 規則

権限エラーが発生した場合、次のように対処します。 

- **オブジェクト ID を持つクライアントには、スコープを通してアクションを実行する権限がありません (コード: AuthorizationFailed)** : リソースを作成しようとするときは、選択したスコープで、リソースへの書き込み権限を持つロールが割り当てられているユーザーとして現在サインインしていることを確認してください。 たとえば、リソース グループ内の仮想マシンを管理するには、リソース グループ (または親スコープ) で[仮想マシン共同作成者](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor)の役割が与えられている必要があります。 各組み込みロールのアクセス許可の一覧については、「[Azure リソースの組み込みロール](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。
- **サポート リクエストを作成する権限がありません**: サポート チケットを作成または更新するときは、現在、[サポート リクエスト 共同作成者](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)などの Microsoft.Support/supportTickets/write permission を持つロールが割り当てられているユーザーとしてサインインしていることを確認してください。
- **これ以上の役割の割り当ては作成できません (コード：RoleAssignmentLimitExceeded)** : 役割を割り当てるには、代わりにグループに役割を割り当てることによって、役割の割り当ての数を減らしてみてください。Azure は、サブスクリプションごとに最大 **2000** の役割の割り当てをサポートします。

Azure RBAC の役割の詳細については、「[Azure RBAC の役割](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。

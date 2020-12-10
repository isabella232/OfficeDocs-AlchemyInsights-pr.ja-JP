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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584213"
---
# <a name="rbac-rules"></a><span data-ttu-id="71fc2-102">RBAC 規則</span><span class="sxs-lookup"><span data-stu-id="71fc2-102">RBAC rules</span></span>

<span data-ttu-id="71fc2-103">権限エラーが発生した場合、次のように対処します。</span><span class="sxs-lookup"><span data-stu-id="71fc2-103">If you get the permission error:</span></span> 

- <span data-ttu-id="71fc2-104">**オブジェクト ID を持つクライアントには、スコープを通してアクションを実行する権限がありません (コード: AuthorizationFailed)** : リソースを作成しようとするときは、選択したスコープで、リソースへの書き込み権限を持つロールが割り当てられているユーザーとして現在サインインしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="71fc2-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="71fc2-105">たとえば、リソース グループ内の仮想マシンを管理するには、リソース グループ (または親スコープ) で[仮想マシン共同作成者](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor)の役割が与えられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="71fc2-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="71fc2-106">各組み込みロールのアクセス許可の一覧については、「[Azure リソースの組み込みロール](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71fc2-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="71fc2-107">**サポート リクエストを作成する権限がありません**: サポート チケットを作成または更新するときは、現在、[サポート リクエスト 共同作成者](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)などの Microsoft.Support/supportTickets/write permission を持つロールが割り当てられているユーザーとしてサインインしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="71fc2-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="71fc2-108">**これ以上の役割の割り当ては作成できません (コード：RoleAssignmentLimitExceeded)** : 役割を割り当てるには、代わりにグループに役割を割り当てることによって、役割の割り当ての数を減らしてみてください。</span><span class="sxs-lookup"><span data-stu-id="71fc2-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="71fc2-109">Azure は、サブスクリプションごとに最大 **2000** の役割の割り当てをサポートします。</span><span class="sxs-lookup"><span data-stu-id="71fc2-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="71fc2-110">Azure RBAC の役割の詳細については、「[Azure RBAC の役割](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71fc2-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

---
title: Outlook でアドインを追加するときに、複数のユーザーにアクセス拒否エラーが発生する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424322"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="3a36d-102">Outlook でアドインを追加するときに、複数のユーザーにアクセス拒否エラーが発生する</span><span class="sxs-lookup"><span data-stu-id="3a36d-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="3a36d-p101">組織のどの管理者に、Outlook 用のアドインをインストールして管理するアクセス許可を持たせるかを指定できます。また、組織のどのユーザーに、自分で使用するアドインをインストールして管理するアクセス許可を持たせるかを指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="3a36d-p101">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook. You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="3a36d-105">詳細については、[「Outlook 用のアドインをインストールおよび管理できる管理者とユーザーを指定する」](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3a36d-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="3a36d-106">ユーザーのアクセス許可が正常に割り当てられたことを確認するには、<Role Name> を検証するロールの名前に置き換え、Exchange Online PowerShell で次のコマンドを実行します:</span><span class="sxs-lookup"><span data-stu-id="3a36d-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="3a36d-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="3a36d-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="3a36d-108">この例は、組織のために Office ストアのアドインをインストールするのに必要なアクセス許可を割り当てた対象を確認する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="3a36d-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="3a36d-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="3a36d-109">PowerShell</span></span>

<span data-ttu-id="3a36d-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="3a36d-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="3a36d-111">Get-ManagementRoleAssignment の結果の [有効なユーザー] 列のエントリを確認します。</span><span class="sxs-lookup"><span data-stu-id="3a36d-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="3a36d-112">構文およびパラメーターの詳細については、「[Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a36d-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 
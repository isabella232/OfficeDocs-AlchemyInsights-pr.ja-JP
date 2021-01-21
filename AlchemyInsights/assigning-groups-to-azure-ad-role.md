---
title: Azure AD 役割へのグループの割り当て
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885801"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="22ec6-102">Azure AD 役割へのグループの割り当て</span><span class="sxs-lookup"><span data-stu-id="22ec6-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="22ec6-103">Azure AD の権限ソースを持つ Azure AD グループを Azure AD 役割に割り当てるには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="22ec6-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="22ec6-104">[新しいグループを作成する] - 新しいグループを作成するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="22ec6-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="22ec6-105">a.</span><span class="sxs-lookup"><span data-stu-id="22ec6-105">a.</span></span> <span data-ttu-id="22ec6-106">**特権役割の管理者** または **全体管理者** の権限を持つ Azure AD 管理センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="22ec6-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="22ec6-107">b.</span><span class="sxs-lookup"><span data-stu-id="22ec6-107">b.</span></span> <span data-ttu-id="22ec6-108">**[Azure Active Directory]、[グループ]、[すべてのグループ]、[新しいグループ]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="22ec6-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="22ec6-109">c.</span><span class="sxs-lookup"><span data-stu-id="22ec6-109">c.</span></span> <span data-ttu-id="22ec6-110">グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="22ec6-110">Create the group.</span></span>

2. <span data-ttu-id="22ec6-111">グループの作成中またはグループの作成後に、役割をグループに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="22ec6-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="22ec6-112">a.</span><span class="sxs-lookup"><span data-stu-id="22ec6-112">a.</span></span> <span data-ttu-id="22ec6-113">グループの作成時にグループに役割を割り当てるには、**[Azure AD 役割をグループに割り当てることができます]** トグルをオンにし、グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="22ec6-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="22ec6-114">b.</span><span class="sxs-lookup"><span data-stu-id="22ec6-114">b.</span></span> <span data-ttu-id="22ec6-115">作成後にグループに役割を割り当てるには、新しく作成したグループの **[割り当てられている役割]** タブに移動し、その役割をグループに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="22ec6-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="22ec6-116">**Azure AD 役割に割り当てられたグループのメンバシップを管理する**</span><span class="sxs-lookup"><span data-stu-id="22ec6-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="22ec6-117">特権を昇格させないために、既定では、特権役割の管理者と全体管理者だけが、役割に割り当てられているグループのメンバシップを変更できます。</span><span class="sxs-lookup"><span data-stu-id="22ec6-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="22ec6-118">ただし、このようなグループに所有者を割り当て、このタスクを委任することもできます。</span><span class="sxs-lookup"><span data-stu-id="22ec6-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="22ec6-119">クラウド グループを Azure AD 役割に割り当てる方法の詳細については、「[クラウド グループに AD 役割を割り当てる](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22ec6-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="22ec6-120">クラウド グループに割り当てられたトラブルシューティングの役割の詳細については、「[クラウド グループに割り当てられた役割のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22ec6-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>






---
title: グループの問題のトラブルシューティング
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886943"
---
# <a name="troubleshoot-group-issues"></a><span data-ttu-id="f5ee2-102">グループの問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="f5ee2-102">Troubleshoot group issues</span></span>

<span data-ttu-id="f5ee2-103">**Azure AD 役割にグループを割り当てる必要がある**</span><span class="sxs-lookup"><span data-stu-id="f5ee2-103">**I need to assign a group to an Azure AD role**</span></span>

<span data-ttu-id="f5ee2-104">Azure Active Directory (AD) グループを Azure AD 役割に割り当てるには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-104">To assign an Azure Active Directory (AD) group to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="f5ee2-105">[新しいグループを作成する] - 新しいグループを作成するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-105">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="f5ee2-106">a.</span><span class="sxs-lookup"><span data-stu-id="f5ee2-106">a.</span></span> <span data-ttu-id="f5ee2-107">特権役割の管理者または全体管理者の権限を持つ Azure AD 管理センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-107">Sign in to the Azure AD admin center with privileged role administrator or global administrator permissions.</span></span> 
    <span data-ttu-id="f5ee2-108">b.</span><span class="sxs-lookup"><span data-stu-id="f5ee2-108">b.</span></span> <span data-ttu-id="f5ee2-109">[Azure Active Directory]、[グループ]、[すべてのグループ]、[新しいグループ] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-109">Select Azure Active Directory > Groups > All groups > New group.</span></span> 
    <span data-ttu-id="f5ee2-110">c.</span><span class="sxs-lookup"><span data-stu-id="f5ee2-110">c.</span></span> <span data-ttu-id="f5ee2-111">グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-111">Create the group.</span></span>

2. <span data-ttu-id="f5ee2-112">グループの作成中またはグループの作成後に、役割をグループに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-112">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="f5ee2-113">a.</span><span class="sxs-lookup"><span data-stu-id="f5ee2-113">a.</span></span> <span data-ttu-id="f5ee2-114">グループの作成時にグループに役割を割り当てるには、[Azure AD 役割をグループに割り当てることができます] トグルをオンにし、グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-114">To assign a role to the group at the time of group creation, switch on the toggle Azure AD roles can be assigned to the group and create the group.</span></span>
    <span data-ttu-id="f5ee2-115">b.</span><span class="sxs-lookup"><span data-stu-id="f5ee2-115">b.</span></span> <span data-ttu-id="f5ee2-116">作成後にグループに役割を割り当てるには、新しく作成したグループの [割り当てられている役割] タブに移動し、その役割をグループに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-116">To assign a role to the group after it has been created, navigate to the Assigned roles tab for the newly created group, and assign the role to the group.</span></span>

<span data-ttu-id="f5ee2-117">**Azure AD 役割に割り当てられたグループのメンバシップを管理する必要がある**</span><span class="sxs-lookup"><span data-stu-id="f5ee2-117">**I need to manage membership of a group that is assigned to Azure AD role**</span></span>

1. <span data-ttu-id="f5ee2-118">特権を昇格させないために、既定では、特権役割の管理者と全体管理者だけが、役割に割り当てられているグループのメンバシップを変更できます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-118">To prevent elevation of privileges, by default, only privileged role administrator and global administrator can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="f5ee2-119">ただし、このようなグループに所有者を割り当て、このタスクを委任することもできます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-119">They can, however, choose to assign an owner for such a group and delegate this task.</span></span> <span data-ttu-id="f5ee2-120">詳細については、「[クラウド グループを使用して、Azure Active Directory の役割の割り当てを管理する](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-120">For more information see, [Use cloud groups to manage role assignments in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span>
2. <span data-ttu-id="f5ee2-121">Azure AD のグループに役割を割り当てる際の一般的な質問とトラブルシューティングのヒントについては、「[クラウド グループに割り当てられた役割のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-121">For common questions and troubleshooting tips for assigning roles to groups in Azure AD, see [Troubleshooting roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>

<span data-ttu-id="f5ee2-122">**動的グループ**</span><span class="sxs-lookup"><span data-stu-id="f5ee2-122">**Dynamic groups**</span></span>

1. <span data-ttu-id="f5ee2-123">組み込みのユーザーの属性が見つからない場合は、その属性がサポートされているプロパティのリストにあることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-123">If you cannot find the built-in user attributes, ensure that the attribute is in the list of supported properties.</span></span>
2. <span data-ttu-id="f5ee2-124">組み込みのデバイスの属性を検索する場合は、属性がデバイスの属性のリストにあることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-124">If you are looking for built-in device attributes, ensure that the attribute is in the list of device attributes</span></span> 
3. <span data-ttu-id="f5ee2-125">組み込みのユーザーの属性およびデバイスの属性に加えて、[拡張属性](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties)も使用できます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-125">In addition to the built-in user and device attributes, you could also use [Extension Attributes](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties).</span></span> <span data-ttu-id="f5ee2-126">オンプレミス Windows Server AD または接続された SaaS アプリケーションから拡張属性を同期すると、規則ビルダーのドロップダウン リストに属性が表示されます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-126">After syncing extension attributes from on-premises Windows Server AD or from a connected SaaS application, the attributes should be visible in the drop-down list of the rule builder.</span></span> <span data-ttu-id="f5ee2-127">カスタム属性名は、PowerShell を使用してユーザーの属性を照会し、属性名を検索することにより、ディレクトリ内で見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-127">The custom attribute name can be found in the directory by querying a user's attribute using PowerShell and searching for the attribute name.</span></span> <span data-ttu-id="f5ee2-128">これらは、規則構文で規則を作成する場合にも使用できます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-128">These could also be used when constructing rules in the rule syntax.</span></span>
4. <span data-ttu-id="f5ee2-129">テナントが適切なライセンスを持っていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-129">Ensure that your tenant has the appropriate license.</span></span> <span data-ttu-id="f5ee2-130">動的グループでは、テナントに Azure AD P1 Premium ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-130">Dynamic groups require the tenant to have an Azure AD P1 Premium license.</span></span> <span data-ttu-id="f5ee2-131">Azure AD ライセンス プランのリストは、[こちら](https://azure.microsoft.com/pricing/details/active-directory/)でアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-131">The list of Azure AD license plans can be accessed [here](https://azure.microsoft.com/pricing/details/active-directory/).</span></span> <span data-ttu-id="f5ee2-132">Enterprise Mobility + Security ライセンス プランは、[こちら](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)でアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-132">Enterprise Mobility + Security licensing plans can be accessed [here](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).</span></span>
5. <span data-ttu-id="f5ee2-133">動的グループを作成するユーザーの役割が、全体管理者、Intune 管理者、グループ管理者、またはユーザー管理者であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-133">Ensure that the role of the user creating the dynamic group is a global administrator, intune administrator, group administrator, or a user administrator.</span></span>
6. <span data-ttu-id="f5ee2-134">グループが入力されるまでしばらくお待ちください。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-134">Please allow time for the group to populate.</span></span> <span data-ttu-id="f5ee2-135">テナントのサイズによっては、最初または規則変更後にグループを入力するのに最大 24 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-135">Depending on the size of your tenant, the group may take up to 24 hours for populating for the first time or after a rule change.</span></span>
7. <span data-ttu-id="f5ee2-136">詳細については、「[動的グループ メンバシップ用の属性ベースの規則の作成](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-136">For more information, see [Create attribute-based rules for dynamic group membership](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).</span></span>

<span data-ttu-id="f5ee2-137">**グループを削除する必要がある**</span><span class="sxs-lookup"><span data-stu-id="f5ee2-137">**I need to delete a group**</span></span>

1. <span data-ttu-id="f5ee2-138">グループは、Azure AD Powershell モジュールの Remove-AzureADGroup コマンドレットを使用してディレクトリから削除できます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-138">Groups can be deleted from the directory using the Remove-AzureADGroup cmdlet in the Azure AD Powershell module.</span></span>
2. <span data-ttu-id="f5ee2-139">Azure AD で同期グループを削除する前に、エラーを回避するために割り当てられたライセンスがすべて削除されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-139">Before attempting to delete a synced group in Azure AD, ensure you have deleted all assigned licenses  to avoid errors.</span></span>
3. <span data-ttu-id="f5ee2-140">グループの削除の詳細については、「[ライセンスが割り当てられているグループの削除](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-140">For more information on deleting groups, see [Deleting a group with an assigned license](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).</span></span>

<span data-ttu-id="f5ee2-141">**削除したグループを復元する必要がある**</span><span class="sxs-lookup"><span data-stu-id="f5ee2-141">**I need to restore a deleted group**</span></span>

1. <span data-ttu-id="f5ee2-142">Office 365 グループが削除された場合、完全な削除が行われる 30 日前までしか復元できません。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-142">If an Office 365 group is deleted, it can only be restored up to 30 days before permanent deletion occurs.</span></span> <span data-ttu-id="f5ee2-143">完全に削除されると、グループは復元できなくなります。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-143">Once permanently deleted, the group can no longer be restored.</span></span> <span data-ttu-id="f5ee2-144">グループの復元の詳細は、[こちら](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-144">Learn more about restoring groups [here](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>
2. <span data-ttu-id="f5ee2-145">この機能は、セキュリティ グループおよび配布グループではサポートされません。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-145">This functionality is not supported for security groups and distribution groups.</span></span>
3. <span data-ttu-id="f5ee2-146">Office 365 グループの復元が承認されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-146">Ensure you are authorized to restore an Office 365 group.</span></span> <span data-ttu-id="f5ee2-147">全体管理者、グループ管理者、ユーザー アカウント管理者、Intune サービス管理者、パートナー レベル 1 または レベル 2 のサポート、およびグループ所有者はグループを復元できます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-147">Global administrators, group administrators, user account administrators, intune service administrators, partner tier1 or tier2 support, and the owner of the group can be able to restore a group.</span></span>
4. <span data-ttu-id="f5ee2-148">動的グループを削除して復元すると、そのグループは新しいグループと見なされ、規則に従って再入力されます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-148">When a dynamic group is deleted and restored, it is seen as a new group and re-populated according to the rule.</span></span> <span data-ttu-id="f5ee2-149">このプロセスには最大 24 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-149">This process might take up to 24 hours.</span></span>
5. <span data-ttu-id="f5ee2-150">削除されたグループの復元の詳細については、「[Azure Active Directory で削除された Office 365 グループを復元する](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-150">For more information on restoring a deleted group, see [Restore a deleted Office 365 group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="f5ee2-151">**グループの有効期限ポリシーの構成**</span><span class="sxs-lookup"><span data-stu-id="f5ee2-151">**Group expiration policy configuration**</span></span>

1. <span data-ttu-id="f5ee2-152">この機能は Office 365 グループのみでサポートされ、セキュリティ グループおよび配布グループではサポートされません。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-152">This functionality is only supported for Office 365 groups, and not for security groups and distribution groups are not supported.</span></span>
2. <span data-ttu-id="f5ee2-153">Office 365 グループの有効期限ポリシーを構成および使用するには、Azure AD Premium ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-153">Configuring and using the expiration policy for Office 365 groups requires an Azure AD Premium license.</span></span>
3. <span data-ttu-id="f5ee2-154">現在、テナント上の Office 365 グループに構成できる有効期限ポリシーは 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-154">Currently, only one expiration policy can be configured for Office 365 groups on a tenant.</span></span>
4. <span data-ttu-id="f5ee2-155">グループを更新できるのは、全体管理者、グループ管理者、ユーザー管理者、およびグループ所有者だけです。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-155">Only Global administrators, group administrators, user administrators, and the owner of the group can be able to renew a group.</span></span>
5. <span data-ttu-id="f5ee2-156">Office 365 グループの有効期限が切れると、そのグループは削除され、完全な削除が行われる 30 日前までしか復元できません。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-156">If an Office 365 group is expired, it is deleted and can only be restored up to 30 days before permanent deletion occurs.</span></span> <span data-ttu-id="f5ee2-157">完全に削除されると、グループは復元できなくなります。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-157">Once permanently deleted, the group can no longer be restored.</span></span> <span data-ttu-id="f5ee2-158">グループの復元の詳細は、[こちら](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-158">Learn more about restoring groups [here](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="f5ee2-159">**アクティビティ ベースの自動更新**</span><span class="sxs-lookup"><span data-stu-id="f5ee2-159">**Activity-based automatic renewal**</span></span>

<span data-ttu-id="f5ee2-160">SharePoint、Outlook、および Teams のユーザー アクティビティによって、グループの自動更新がトリガーされます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-160">User activities from SharePoint, Outlook and Teams can trigger group automatic renewal.</span></span> <span data-ttu-id="f5ee2-161">アクティビティは、グループが期限切れになる 35 日前に確認されます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-161">Activities are checked at 35 days before a group expires.</span></span> <span data-ttu-id="f5ee2-162">現在のグループの有効期限中にアクティビティが発生した場合、グループは自動的に更新され、メール通知はグループ所有者に送信されません。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-162">If there is activity during the current group lifecycle, the group will be automatically renewed and email notification won't be sent out to group owners.</span></span>

<span data-ttu-id="f5ee2-163">**期限切れグループの通知タイミング**</span><span class="sxs-lookup"><span data-stu-id="f5ee2-163">**Notification timing for expired groups**</span></span>

1. <span data-ttu-id="f5ee2-164">メール通知は、グループの有効期限の 30 日前、15 日前、および 1 日前に Office 365 グループ所有者に送信されます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-164">Email notifications are sent to the Office 365 group owners 30 days, 15 days, and 1 day prior to expiration of the group.</span></span>
2. <span data-ttu-id="f5ee2-165">最初に有効期限を設定したとき、有効期限の間隔より古いグループは、有効期限まで 35 日に設定されます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-165">When you first set up expiration, any groups that are older than the expiration interval are set to 35 days until expiration.</span></span>
3. <span data-ttu-id="f5ee2-166">グループの有効期限は、ポリシーの更新日ではなく、グループの更新日に基づいて計算されます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-166">Group expiration date is calculated based on the group’s renewal date, not based on the policy updated date.</span></span> <span data-ttu-id="f5ee2-167">有効期限ポリシーが更新されても、有効期限は変更されません。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-167">If the expiration policy is updated, the expiration date will not change.</span></span>
4. <span data-ttu-id="f5ee2-168">詳細については、「[グループの有効期限ポリシーと更新メール](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle)」および「[削除した Office 365 グループを Azure Active Directory に復元する](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-168">For more information see, [Group Expiration policy and renewal emails](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) and [Restore a deleted Office 365 group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="f5ee2-169">**グループを作成する権限**</span><span class="sxs-lookup"><span data-stu-id="f5ee2-169">**Permission to create a group**</span></span>

<span data-ttu-id="f5ee2-170">新しいグループを作成する権限があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-170">Ensure that you are authorized to create a new group.</span></span> <span data-ttu-id="f5ee2-171">グローバル管理者は、Azure ポータルまたはアクセス パネルでグループの作成を無効にできます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-171">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="f5ee2-172">新しいグループを作成したり、適切な権限を付与したりするには、管理者が必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-172">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

1. [<span data-ttu-id="f5ee2-173">Azure portal で新しいグループを作成し、メンバを追加する</span><span class="sxs-lookup"><span data-stu-id="f5ee2-173">Create a new group and add members in Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [<span data-ttu-id="f5ee2-174">Powershell MS Online でグループを作成する</span><span class="sxs-lookup"><span data-stu-id="f5ee2-174">Create groups in Powershell MSOnline</span></span>](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [<span data-ttu-id="f5ee2-175">Powershell でグループの作成を無効にする</span><span class="sxs-lookup"><span data-stu-id="f5ee2-175">Disable groups creation in Powershell</span></span>](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [<span data-ttu-id="f5ee2-176">Office 365 でグループを作成できるユーザーを管理する</span><span class="sxs-lookup"><span data-stu-id="f5ee2-176">Manage who can create groups in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [<span data-ttu-id="f5ee2-177">Powershell を介した Office 365 ウェルカム通知を無効にする</span><span class="sxs-lookup"><span data-stu-id="f5ee2-177">Disable Office 365 welcome notification via Powershell</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [<span data-ttu-id="f5ee2-178">Azure AD 管理者の役割</span><span class="sxs-lookup"><span data-stu-id="f5ee2-178">Azure AD administrative roles</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

<span data-ttu-id="f5ee2-179">**グループ作成権限を管理する**</span><span class="sxs-lookup"><span data-stu-id="f5ee2-179">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="f5ee2-180">全体管理者は、**[すべてのグループ]、[全般 (設定)]** の順に移動し、**[ユーザーは Azure portal でセキュリティ グループを作成できます]** または **[ユーザーは Azure portal で Office 365 グループを作成できます]** を設定することにより、セキュリティ上の理由でグループ作成のアクセス許可、Azure portal、またはアクセス パネルで作成された Office 365 グループを管理できます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-180">Global administrators can manage group creation permissions for security or Office 365 groups created in the Azure portal or Access Panel, by setting **Users can create security groups in Azure portals** or **Users can create Office 365 groups in Azure portals** settings in **All groups > General (Settings)**.</span></span>
2. <span data-ttu-id="f5ee2-181">Azure AD P1 Premium ライセンスをお持ちの場合は、グループの作成を制限してユーザーのグループを選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-181">You can also restrict group creation to select a group of users if you have an Azure AD P1 Premium license.</span></span>

<span data-ttu-id="f5ee2-182">**新しい Office 365 グループ メンバーのウェルカム通知を無効にする**</span><span class="sxs-lookup"><span data-stu-id="f5ee2-182">**Disabling welcome notification for new members of an Office 365 group**</span></span>

<span data-ttu-id="f5ee2-183">Office 365 グループに追加されたユーザーに送信されるウェルカム通知を無効にするには、Powershell で `UnifiedGroupWelcomeMessageEnabled` を **False** に設定します。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-183">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting `UnifiedGroupWelcomeMessageEnabled` to **False** in Powershell.</span></span> <span data-ttu-id="f5ee2-184">この設定については、[こちら](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-184">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).</span></span>














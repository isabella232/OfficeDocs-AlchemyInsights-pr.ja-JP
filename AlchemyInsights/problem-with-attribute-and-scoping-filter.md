---
title: 属性とスコープ フィルターの問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50484065"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="ae826-102">属性とスコープ フィルターの問題</span><span class="sxs-lookup"><span data-stu-id="ae826-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="ae826-103">**競合する UPN 値の問題**</span><span class="sxs-lookup"><span data-stu-id="ae826-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="ae826-104">Workday to AD ユーザーのプロビジョニング Workday to AD ユーザーのプロビジョニングは、エラーメッセージ **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique** を表示します。</span><span class="sxs-lookup"><span data-stu-id="ae826-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="ae826-105">追加/変更のために提供された UPN 値がフォレスト全体で一意ではないため、操作は失敗しました。</span><span class="sxs-lookup"><span data-stu-id="ae826-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="ae826-106">エラーの詳細: **CONSTRAINT_ATT_TYPE - userPrincipalName**。</span><span class="sxs-lookup"><span data-stu-id="ae826-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="ae826-107">Workday コネクタ がAD ユーザー アカウントの作成時に設定しようとしている **userPrincipalName** 値は、ターゲット AD ドメインにすでに存在します。</span><span class="sxs-lookup"><span data-stu-id="ae826-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="ae826-108">これは、(1) ユーザーがすでに存在し、ユーザーの一致する ID チェックが失敗したか、(2) UPN 生成ルールが競合する値を生成したことを意味します。</span><span class="sxs-lookup"><span data-stu-id="ae826-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="ae826-109">推奨される解決手順は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ae826-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="ae826-110">ユーザーがすでに存在し、一致する ID チェックで Workday アカウントを Active Directory アカウントにリンクできなかった場合は、Workday と AD の両方で一致する ID 属性 (通常は **employeeID**) が完全に一致するかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="ae826-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="ae826-111">一致するものがない場合は、データの問題を修正する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae826-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="ae826-112">たとえば、Workday の EmployeeID が 001052 で、AD の EmployeeID が 1052 の場合、プロビジョニング エンジンは、2 つのアカウントのリンクに失敗し、既存のユーザーを作成しようとします。</span><span class="sxs-lookup"><span data-stu-id="ae826-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="ae826-113">この場合は、AD の **EmployeeID** 値を変更して、先行のゼロを含めて 001052 にすることで解決できます。</span><span class="sxs-lookup"><span data-stu-id="ae826-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="ae826-114">UPN 生成式が一意の値を生成していない場合は、重複排除関数 **SelectUniqueValue** を使用して、毎回一意の値を生成することを検討してください。</span><span class="sxs-lookup"><span data-stu-id="ae826-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="ae826-115">**Workday to AD User Provisioningは、AD ユーザー アカウントのマネージャー属性値を設定しません**</span><span class="sxs-lookup"><span data-stu-id="ae826-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="ae826-116">Workday to AD User Provisioning ジョブは、AD ユーザー アカウントの **マネージャー** 属性値を設定していません。</span><span class="sxs-lookup"><span data-stu-id="ae826-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="ae826-117">この動作が見られる場合、次の 2 つのシナリオが考えられます。</span><span class="sxs-lookup"><span data-stu-id="ae826-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="ae826-118">Manager がスコープ内にないため、Workday のマネージャーに対応する AD ユーザー アカウントに解決できません。</span><span class="sxs-lookup"><span data-stu-id="ae826-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="ae826-119">**複数の AD ドメイン** のシナリオでは、Workday のマネージャーはユーザーと同じドメインに存在しません。</span><span class="sxs-lookup"><span data-stu-id="ae826-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="ae826-120">問題を解決するには、次の手順を試してください。</span><span class="sxs-lookup"><span data-stu-id="ae826-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="ae826-121">スコープ フィルターを定義した場合は、最初にマネージャーがスコープ内にあるかどうか、およびマネージャーがスコープ句を満たしているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="ae826-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="ae826-122">マネージャがスコープ フィルターを満たさない場合は、フィルタを変更して、マネージャもプロビジョニング操作の範囲内にあるようにします。</span><span class="sxs-lookup"><span data-stu-id="ae826-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="ae826-123">複数の AD ドメインがある場合、コネクタには、クロス ドメイン マネージャー参照を解決できないという既知の制限があります。</span><span class="sxs-lookup"><span data-stu-id="ae826-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="ae826-124">自動プロビジョニング用の Workday の構成の詳細については、「[チュートリアル: Workday を構成し、自動ユーザー プロビジョニングに対応させる](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae826-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>














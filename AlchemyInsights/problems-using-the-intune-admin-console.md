---
title: Intune 管理コンソールの使用に関する問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728292"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="2094a-102">Intune 管理コンソールの使用に関する問題</span><span class="sxs-lookup"><span data-stu-id="2094a-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="2094a-103">**Intune 管理コンソール内を移動すると、"アクセスが拒否されました" と表示されます。**</span><span class="sxs-lookup"><span data-stu-id="2094a-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="2094a-104">Intune カスタム ロールのメンバーである場合は、Intune ライセンスまたは Enterprise Mobility Suite (EMS) ライセンスが自分のアカウントに割り当てられていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="2094a-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="2094a-105">Configuration Manager を使用してデバイスを管理している場合、自分が Configuration Manager MDM の Intune ユーザー コレクションに含まれていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="2094a-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="2094a-106">Intune のロール ブレードで、適切なロールベースの管理制御 (RBAC) が自分に割り当てられていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="2094a-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="2094a-107">使用しているグループが配布リストではないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="2094a-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="2094a-108">Azure ポータルの Intune では、Azure Active Directory セキュリティ グループに属するユーザー アカウントのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="2094a-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="2094a-109">自分のグループを確認するために、Azure ポータル > [**Intune**] > [**グループ**] または Azure ポータル > [**Azure Active Directory**] の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="2094a-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="2094a-110">**ユーザーに割り当てられているアクセス権限の数が、割り当てられている Intune のロールに対して多すぎる**</span><span class="sxs-lookup"><span data-stu-id="2094a-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="2094a-111">ユーザーに、[**Intune**] > [**Intune のロール**] > [**自分のアクセス権限**] > [**エクスポート**] の順に移動して、付与されているアクセス許可を確認するよう依頼します。</span><span class="sxs-lookup"><span data-stu-id="2094a-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="2094a-112">**ロールにスコープ グループを追加しましたが、そのロールのユーザーには他のユーザーまたはデバイスが表示されます。**</span><span class="sxs-lookup"><span data-stu-id="2094a-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="2094a-113">スコープ グループは、ユーザーやデバイスを除外しません。</span><span class="sxs-lookup"><span data-stu-id="2094a-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="2094a-114">スコープ グループ:</span><span class="sxs-lookup"><span data-stu-id="2094a-114">Scope groups:</span></span>

- <span data-ttu-id="2094a-115">ユーザーがポリシーまたはアプリケーションを割り当てる相手のユーザーを制限します。</span><span class="sxs-lookup"><span data-stu-id="2094a-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="2094a-116">特定のユーザーのみがデバイスでリモート タスクを実行できるようにします。</span><span class="sxs-lookup"><span data-stu-id="2094a-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="2094a-117">スコープ グループの詳細については、「[Microsoft Intune のロールベースのアクセス制御 (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="2094a-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="2094a-118">**ユーザーを Intune のロールに追加しましたが、このユーザーは引き続き Intune 管理コンソールにフルアクセスできます。**</span><span class="sxs-lookup"><span data-stu-id="2094a-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="2094a-119">Azure ポータルで [Intune]、[**ユーザー**] の順に移動し、このユーザーが Azure ポータルで次のいずれのロールにも割り当てられていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="2094a-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="2094a-120">全体管理者</span><span class="sxs-lookup"><span data-stu-id="2094a-120">Global administrator</span></span>
- <span data-ttu-id="2094a-121">Intune サービス管理者</span><span class="sxs-lookup"><span data-stu-id="2094a-121">Intune service administrator</span></span>
- <span data-ttu-id="2094a-122">SharePoint 管理者</span><span class="sxs-lookup"><span data-stu-id="2094a-122">SharePoint administrator</span></span>

<span data-ttu-id="2094a-123">詳細については、「[Microsoft Intune のロールベースのアクセス制御 (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="2094a-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="2094a-124">**アクセスに関する問題**</span><span class="sxs-lookup"><span data-stu-id="2094a-124">**Access Issues**</span></span>

<span data-ttu-id="2094a-125">詳細については、「[Office 365、Azure、または Intune にサインインできない](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2094a-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>
---
title: アクセスの制限
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7769"
ms.openlocfilehash: 8af9546f219474e2382cd2436470385bf3ad31e8
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015071"
---
# <a name="restricting-access"></a><span data-ttu-id="ba152-102">アクセスの制限</span><span class="sxs-lookup"><span data-stu-id="ba152-102">Restricting access</span></span>

1. <span data-ttu-id="ba152-103">アプリケーションへのアクセスを制限する方法については、「[方法: Azure AD アプリを Azure AD テナント内の一連のユーザーに制限する](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba152-103">For information on how to restrict access to an application, see [How to: Restrict your Azure AD app to a set of users in an Azure AD tenant](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users).</span></span>
1. <span data-ttu-id="ba152-104">アプリケーションの権限を確認および管理する方法を学びます。</span><span class="sxs-lookup"><span data-stu-id="ba152-104">Learn how to review and manage application permissions.</span></span> <span data-ttu-id="ba152-105">[Azure Active Directory で特権が過剰なアプリケーションや疑わしいアプリケーションに対してアクションを実行する](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-application-permissions#control-access-to-an-application)と、シナリオに応じてアプリケーションを保護するために実行できるさまざまなアクションが提供されます。</span><span class="sxs-lookup"><span data-stu-id="ba152-105">[Take action on overprivileged or suspicious applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-application-permissions#control-access-to-an-application) provides different actions you can take to secure your application according to the scenario.</span></span> <span data-ttu-id="ba152-106">これらのアクションは、ユーザーまたは管理者の同意によって Azure Active Directory (Azure AD) テナントに追加されたすべてのアプリケーションに適用されます。</span><span class="sxs-lookup"><span data-stu-id="ba152-106">These actions apply to all applications that were added to your Azure Active Directory (Azure AD) tenant via user or admin consent.</span></span>
1. <span data-ttu-id="ba152-107">「[Azure Active Directory でのアプリのユーザー割り当ての管理](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal#configure-an-application-to-require-user-assignment)」では、Azureポータル内から、または PowerShell を使用して、Azure Active Directory (Azure AD) のエンタープライズ アプリケーションにユーザーとグループを割り当てる方法を示します。</span><span class="sxs-lookup"><span data-stu-id="ba152-107">[Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal#configure-an-application-to-require-user-assignment) shows you how to assign users, and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell.</span></span> <span data-ttu-id="ba152-108">ユーザーをアプリケーションに割り当てると、そのアプリケーションはユーザーの [マイ アプリ] に表示され、簡単にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="ba152-108">When you assign a user to an application, the application appears in the user's My Apps for easy access.</span></span> <span data-ttu-id="ba152-109">アプリケーションが役割を公開している場合は、特定の役割をユーザーに割り当てることもできます。</span><span class="sxs-lookup"><span data-stu-id="ba152-109">If the application exposes roles, you can also assign a specific role to the user.</span></span>
    - <span data-ttu-id="ba152-110">ユーザーとグループの割り当ての詳細については、「[条件付きアクセス: ユーザーとグループ](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-users-groups)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba152-110">For more information on User and Group assignment see [Conditional Access: Users and groups](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-users-groups).</span></span>

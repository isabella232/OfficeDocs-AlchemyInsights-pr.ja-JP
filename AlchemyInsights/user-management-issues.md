---
title: ユーザー管理に関する問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038299"
---
# <a name="user-management-issues"></a><span data-ttu-id="d7827-102">ユーザー管理に関する問題</span><span class="sxs-lookup"><span data-stu-id="d7827-102">User management issues</span></span>

<span data-ttu-id="d7827-103">**[ユーザー割り当てが必要] を無効に(このプロパティを [いいえ] に設定)した場合、 アプリケーションに現在割り当てられているユーザーはどうなりますか?**</span><span class="sxs-lookup"><span data-stu-id="d7827-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="d7827-104">「**ユーザー割り当てが必要**」を無効にしても、現在割り当てられているユーザーには影響しません。</span><span class="sxs-lookup"><span data-stu-id="d7827-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="d7827-105">このプロパティを無効にすると、すべてのユーザーがアプリケーションにアクセスできるようになるのみです。</span><span class="sxs-lookup"><span data-stu-id="d7827-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="d7827-106">リストにあるすべてのユーザーと、アプリケーションのグループに割り当てられているユーザーは引き続き有効です。</span><span class="sxs-lookup"><span data-stu-id="d7827-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="d7827-107">アプリを特定の一連のユーザーに制限する方法については、「- [Azure AD アプリを一連のユーザーに制限する - Microsoft ID プラットフォーム | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7827-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="d7827-108">Azure ポータル内からまたは PowerShell を使用して、Azure Active Directory (Azure AD) のエンタープライズ アプリケーションにユーザーとグループを割り当てる方法については、「[Azure Active Directory でのアプリのユーザー割り当ての管理](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7827-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="d7827-109">アプリケーションの作成と管理のアクセス許可を委任するには、「[アプリケーション管理を委任する](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles) - Azure AD | Microsoft Docs」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7827-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="d7827-110">**特定のエンタープライズ アプリをユーザーから非表示にする** - 次の手順にしたがって、[**MyApps**] ウィンドウからすべての Microsoft 365 アプリを非表示にします。</span><span class="sxs-lookup"><span data-stu-id="d7827-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="d7827-111">アプリは引き続き Office 365 ポータルに表示されます。</span><span class="sxs-lookup"><span data-stu-id="d7827-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="d7827-112">ディレクトリのグローバル管理者として Azure ポータルにサインインします。</span><span class="sxs-lookup"><span data-stu-id="d7827-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="d7827-113">[**Azure Active Directory**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7827-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="d7827-114">[**ユーザー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7827-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="d7827-115">[**ユーザー設定**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7827-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="d7827-116">[**エンタープライズ アプリケーション]** で、[ **エンド ユーザーがアプリケーションを起動して表示する方法を、管理する] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="d7827-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="d7827-117">ユーザーが **Office 365 ポータルで Office 365 アプリのみしか表示されない** 場合は、[**はい**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d7827-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="d7827-118">**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d7827-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="d7827-119">詳細については、「[Azure AD のユーザーエクスペリエンスからエンタープライズ アプリケーションを非表示にする | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7827-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="d7827-120">SaaS (Software as a Service) アプリを多くの組織に提供している場合、任意の Azure Active Directory (Azure AD) テナントからのサインインを承諾するようにアプリを構成することができます。</span><span class="sxs-lookup"><span data-stu-id="d7827-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="d7827-121">これは、"アプリケーションをマルチテナントにする" 構成と呼ばれています。</span><span class="sxs-lookup"><span data-stu-id="d7827-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="d7827-122">Azure AD テナントのユーザーは、自分のアカウントをアプリで使用することに同意した後、アプリにサインインできます。</span><span class="sxs-lookup"><span data-stu-id="d7827-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="d7827-123">詳細については、「[Azure AD ユーザーにサインインするアプリをビルドする - Microsoft ID プラットフォーム | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7827-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="d7827-124">**アプリケーションに割り当てられたエンド ユーザーがアプリケーションにアクセスするには**</span><span class="sxs-lookup"><span data-stu-id="d7827-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="d7827-125">エンタープライズ アプリケーション ブレードの各アプリには、エンドユーザーがアクセスするためのリンクがあります。</span><span class="sxs-lookup"><span data-stu-id="d7827-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="d7827-126">ユーザーは、**Myapps** ポータルから簡単な方法でアプリにアクセスすることもできます。</span><span class="sxs-lookup"><span data-stu-id="d7827-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="d7827-127">**ユーザーが使用しているアプリケーションおよびアプリケーションの種類を知りたい場合**</span><span class="sxs-lookup"><span data-stu-id="d7827-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="d7827-128">**portal.azure.com > Azure Active Directory > サインイン > レポートのダウンロード** から、過去 30 日間のサインインレポートをダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="d7827-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="d7827-129">[テナント全体の管理者の同意をアプリケーションに付与する](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent)方法と、[エンドユーザーがアプリケーションに同意する方法を構成する](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)方法について学びます。 </span><span class="sxs-lookup"><span data-stu-id="d7827-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="d7827-130">[同意の機能の仕方](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)を理解し、[アプリケーションへの同意を管理](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)します。</span><span class="sxs-lookup"><span data-stu-id="d7827-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>



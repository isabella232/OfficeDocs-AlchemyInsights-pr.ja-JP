---
title: user の作成
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751142"
---
# <a name="create-user"></a><span data-ttu-id="4dc56-102">ユーザーを作成する</span><span class="sxs-lookup"><span data-stu-id="4dc56-102">Create user</span></span>

<span data-ttu-id="4dc56-103">**お知らせ:**</span><span class="sxs-lookup"><span data-stu-id="4dc56-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="4dc56-104">[2021 年 1 月 4 日以降、Google は WebView サインインのサポートを廃止します](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)。</span><span class="sxs-lookup"><span data-stu-id="4dc56-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="4dc56-105">互換性のテストに関する [Google のガイダンス](https://go.microsoft.com/fwlink/?linkid=2157323)に従って、アプリが影響を受けるかどうかをテストします。</span><span class="sxs-lookup"><span data-stu-id="4dc56-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="4dc56-106">コンシューマー向けの Google アカウントでユーザーにサインインするときは、必ずシステム WebView またはシステム ブラウザーを使用してください。</span><span class="sxs-lookup"><span data-stu-id="4dc56-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="4dc56-107">詳細については、「[Chrome ブラウザのみを使用してアプリケーションにサインインする際の問題](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4dc56-107">For more information, see [Issues signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="4dc56-108">**Azure AD ディレクトリに新しいユーザーを作成できません**</span><span class="sxs-lookup"><span data-stu-id="4dc56-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="4dc56-109">新しい標準ユーザーを作成する権限があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="4dc56-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="4dc56-110">新しい標準ユーザーを作成できるのは、Azure Active Directory (AD) のグローバル管理者またはユーザー管理者のみです。</span><span class="sxs-lookup"><span data-stu-id="4dc56-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="4dc56-111">これらの役割のいずれにも属していない場合は、管理者にこれらの役割のいずれかに追加してもらうか、新しいユーザー アカウントを作成するように依頼してください。</span><span class="sxs-lookup"><span data-stu-id="4dc56-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="4dc56-112">ユーザー名が Azure AD で確認済みのドメインにあることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="4dc56-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="4dc56-113">Azure AD に確認済みのカスタム ドメイン名がない場合は、\*.onmicrosoft.com で終わる Azure AD イニシャル ドメインを使用できます。</span><span class="sxs-lookup"><span data-stu-id="4dc56-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="4dc56-114">ユーザー名が、オンプレミス AD から Azure AD にフェデレーションされていないドメインにあることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="4dc56-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="4dc56-115">オンプレミスからフェデレーションされたドメイン名でユーザーをクラウドに追加することはできません。</span><span class="sxs-lookup"><span data-stu-id="4dc56-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="4dc56-116">新しいユーザーに割り当てるユーザー名が、他のユーザーまたは連絡先にないことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="4dc56-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="4dc56-117">ユーザー名は、Azure AD 全体で一意である必要があります。</span><span class="sxs-lookup"><span data-stu-id="4dc56-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="4dc56-118">「[Azure Active Directory でのロールと管理者](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4dc56-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="4dc56-119">Azure AD の[ドメイン名](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="4dc56-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="4dc56-120">[監査ログ](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)を確認して、アクションを実行したユーザーとタイミングなど、最近作成または削除されたユーザーに関する詳細情報を確認します。</span><span class="sxs-lookup"><span data-stu-id="4dc56-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="4dc56-121">新しいユーザーの追加の詳細については、「[Azure portal を使用して Azure AD に新しいユーザーを作成する](/azure/active-directory/active-directory-users-create-azure-portal)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4dc56-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="4dc56-122">[Azure AD での管理者の役割](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): Azure Active Directory での管理者の役割のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="4dc56-122">[Azure AD administrative roles](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="4dc56-123">[Azure AD PowerShell を使用して新しいユーザーを作成する](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)こともできます。</span><span class="sxs-lookup"><span data-stu-id="4dc56-123">You can also [use Azure AD PowerShell to create a new user](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>

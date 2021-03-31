---
title: API アクセス許可と同意の手順
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405827"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="69b1d-102">API アクセス許可と同意の手順</span><span class="sxs-lookup"><span data-stu-id="69b1d-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="69b1d-103">アプリから Microsoft Graph のデータにアクセスする場合、ユーザーまたは管理者は、同意のプロセスを通してそのアプリに正しいアクセス許可を付与する必要があります。</span><span class="sxs-lookup"><span data-stu-id="69b1d-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="69b1d-104">[Microsoft Graph のアクセス許可リファレンス](https://docs.microsoft.com/graph/permissions-reference)では、Microsoft Graph API の各主要なセットに関連付けられているアクセス許可について説明します。</span><span class="sxs-lookup"><span data-stu-id="69b1d-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="69b1d-105">また、アクセス許可の使用方法に関するガイダンスを提供しています。</span><span class="sxs-lookup"><span data-stu-id="69b1d-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="69b1d-106">**サービス プリンシパルを設定または更新する**</span><span class="sxs-lookup"><span data-stu-id="69b1d-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="69b1d-107">[serviceprincipal の作成](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - この記事では、新しい servicePrincipal オブジェクトを作成する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="69b1d-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="69b1d-108">[ポータルを使用して Azure AD アプリとサービス プリンシパルを作成する](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - この記事では、役割ベースのアクセス制御で使用できる新しい Azure Active Directory (Azure AD) アプリケーションとサービス プリンシパルを作成する方法が示されています。</span><span class="sxs-lookup"><span data-stu-id="69b1d-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="69b1d-109">[AzureAD のアプリとサービスプリンシパル](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - この記事では、Azure Active Directory でのアプリケーションの登録、アプリケーション オブジェクト、およびサービス プリンシパルについて、それらが何であるか、どのように使用されるか、お互いがどのように関連しているかについて説明しています。</span><span class="sxs-lookup"><span data-stu-id="69b1d-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="69b1d-110">**アプリ登録を追加または更新し、管理者の同意を提供します**</span><span class="sxs-lookup"><span data-stu-id="69b1d-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="69b1d-111">[アプリ登録の作成](https://docs.microsoft.com/graph/api/application-post-applications) - この記事では、新しいアプリケーション オブジェクトを作成する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="69b1d-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="69b1d-112">[アプリ登録の更新 - API 権限](https://docs.microsoft.com/graph/api/application-update) - この記事では、アプリケーション オブジェクトのプロパティを更新する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="69b1d-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="69b1d-113">[管理者の同意を提供する](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - 管理者の同意と一般的な同意については、管理者が明示的に同意を与える必要があります。</span><span class="sxs-lookup"><span data-stu-id="69b1d-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="69b1d-114">[RBAC (ベータ版)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - 単一の役割割り当てで複数のプリンシパルと複数の範囲をサポートする Microsoft 365 RBAC プロバイダーの統合された役割定義と役割割り当てのための役割管理コンテナー。</span><span class="sxs-lookup"><span data-stu-id="69b1d-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="69b1d-115">これは、*rbacApplication* リソース タイプとは異なります。</span><span class="sxs-lookup"><span data-stu-id="69b1d-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="69b1d-116">Microsoft Intune は、そのような RBAC プロバイダーの一例です。</span><span class="sxs-lookup"><span data-stu-id="69b1d-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="69b1d-117">Intune での役割の割り当てには、プリンシパルの配列と範囲グループの配列を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="69b1d-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="69b1d-118">**これはベータ版です。つまり、まだ開発中であり、本番環境での使用は推奨されていません。**</span><span class="sxs-lookup"><span data-stu-id="69b1d-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>

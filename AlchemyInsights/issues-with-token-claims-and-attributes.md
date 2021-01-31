---
title: トークンの要求と属性に関する問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036130"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="45d69-102">トークンの要求と属性に関する問題</span><span class="sxs-lookup"><span data-stu-id="45d69-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="45d69-103">**トークンの要求の更新、構成、または削除**</span><span class="sxs-lookup"><span data-stu-id="45d69-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="45d69-104">Azure Active Directory (Azure AD) を使用することで、アプリを認証した後に受け取るレスポンス トークンの[役割の要求における要求の種類をカスタマイズする](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)ことができます。</span><span class="sxs-lookup"><span data-stu-id="45d69-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="45d69-105">アプリケーションの開発者は、Azure AD アプリケーションにオプションの要求を使用することで、アプリケーションに送信されるトークンに含める要求を指定できます。</span><span class="sxs-lookup"><span data-stu-id="45d69-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="45d69-106">詳細については、「[アプリにオプションの要求を提供する](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45d69-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="45d69-107">[Azure Active Directory を使用してアプリケーションのグループ要求を構成する](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)。</span><span class="sxs-lookup"><span data-stu-id="45d69-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="45d69-108">アプリケーションでシームレスなシングル サインオンを使用する場合、「[エンタープライズ アプリケーションの SAML トークンで発行された要求のカスタマイズ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45d69-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="45d69-109">**要求の属性のマッピング**</span><span class="sxs-lookup"><span data-stu-id="45d69-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="45d69-110">PowerShell を使用して要求のマッピング ポリシーを構成するには、「[Customize claims emitted in tokens for a specific app in a tenant (Preview) (テナント内の特定のアプリのトークンで発行される要求をカスタマイズする (プレビュー))](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45d69-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="45d69-111">ディレクトリ スキーマ拡張属性は、ユーザー オブジェクトや、グループ、テナントの詳細、サービス プリンシパルなどのその他のディレクトリ オブジェクトの追加データを Azure Active Directory に保存する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="45d69-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="45d69-112">アプリケーションに要求を発行するために使用できるのは、ユーザー オブジェクトの拡張属性だけです。</span><span class="sxs-lookup"><span data-stu-id="45d69-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="45d69-113">「[Using directory schema extension attributes in claims (要求でのディレクトリ スキーマ拡張属性の使用)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)」では、トークンの要求でアプリケーションへのユーザー データの送信にディレクトリ スキーマ拡張属性を使用する方法について説明しています。</span><span class="sxs-lookup"><span data-stu-id="45d69-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="45d69-114">トークンの要求に関する詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45d69-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="45d69-115">アクセス トークンでの要求</span><span class="sxs-lookup"><span data-stu-id="45d69-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="45d69-116">Id_token での要求</span><span class="sxs-lookup"><span data-stu-id="45d69-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="45d69-117">Azure AD B2C で発行された ID トークンやアクセス トークンで想定される[要求](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims)</span><span class="sxs-lookup"><span data-stu-id="45d69-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="45d69-118">SAML トークンの要求のリファレンス</span><span class="sxs-lookup"><span data-stu-id="45d69-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)

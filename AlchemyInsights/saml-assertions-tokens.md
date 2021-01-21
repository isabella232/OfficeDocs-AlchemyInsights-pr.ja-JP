---
title: SAML アサーション (トークン)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885823"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="e7e5a-102">SAML アサーション (トークン)</span><span class="sxs-lookup"><span data-stu-id="e7e5a-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="e7e5a-103">Security Assertions Markup Language (SAML) トークンは、クレームの XML 表現です。</span><span class="sxs-lookup"><span data-stu-id="e7e5a-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="e7e5a-104">既定では、フェデレーション セキュリティ シナリオで Windows Communication Foundation (WCF) が使用する SAML トークンが発行されます。</span><span class="sxs-lookup"><span data-stu-id="e7e5a-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="e7e5a-105">詳細については、「[SAML トークンとクレーム](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7e5a-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="e7e5a-106">Microsoft ID プラットフォームは、各認証フローの処理で複数の種類のセキュリティ トークンを発行します。</span><span class="sxs-lookup"><span data-stu-id="e7e5a-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="e7e5a-107">[SAML トークン クレーム リファレンス](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)には、SAML 2.0 トークンの形式、セキュリティ特性、および内容が記載されています。</span><span class="sxs-lookup"><span data-stu-id="e7e5a-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="e7e5a-108">トークンの有効期限を構成する方法については、「[Microsoft ID プラットフォームで構成可能なトークンの有効期限](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」のガイダンスに従ってください。</span><span class="sxs-lookup"><span data-stu-id="e7e5a-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="e7e5a-109">Azure AD SAML トークン暗号化を構成する方法については、[この記事](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption)で説明されている手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="e7e5a-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="e7e5a-110">Azure AD では、証明書署名オプションと証明書署名アルゴリズムをセットアップできます。</span><span class="sxs-lookup"><span data-stu-id="e7e5a-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="e7e5a-111">詳細については、「[Azure Active Directory のギャラリー アプリ用の SAML トークンの高度な証明書署名オプション](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7e5a-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

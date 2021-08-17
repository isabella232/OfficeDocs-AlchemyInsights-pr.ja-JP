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
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109245"
---
# <a name="saml-assertions-tokens"></a>SAML アサーション (トークン)

1. Security Assertions Markup Language (SAML) トークンは、クレームの XML 表現です。 既定では、フェデレーション セキュリティ シナリオで Windows Communication Foundation (WCF) が使用する SAML トークンが発行されます。 詳細については、「[SAML トークンとクレーム](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)」を参照してください。
2. Microsoft ID プラットフォームは、各認証フローの処理で複数の種類のセキュリティ トークンを発行します。 [SAML トークン クレーム リファレンス](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)には、SAML 2.0 トークンの形式、セキュリティ特性、および内容が記載されています。
3. トークンの有効期限を構成する方法については、「[Microsoft ID プラットフォームで構成可能なトークンの有効期限](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」のガイダンスに従ってください。
4. Azure AD SAML トークン暗号化を構成する方法については、[この記事](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption)で説明されている手順に従ってください。
5. Azure AD では、証明書署名オプションと証明書署名アルゴリズムをセットアップできます。 詳細については、「[Azure Active Directory のギャラリー アプリ用の SAML トークンの高度な証明書署名オプション](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)」を参照してください。

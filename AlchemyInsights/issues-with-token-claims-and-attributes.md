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
# <a name="issues-with-token-claims-and-attributes"></a>トークンの要求と属性に関する問題

**トークンの要求の更新、構成、または削除**

1. Azure Active Directory (Azure AD) を使用することで、アプリを認証した後に受け取るレスポンス トークンの[役割の要求における要求の種類をカスタマイズする](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)ことができます。
2. アプリケーションの開発者は、Azure AD アプリケーションにオプションの要求を使用することで、アプリケーションに送信されるトークンに含める要求を指定できます。 詳細については、「[アプリにオプションの要求を提供する](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)」を参照してください。
3. [Azure Active Directory を使用してアプリケーションのグループ要求を構成する](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)。
4. アプリケーションでシームレスなシングル サインオンを使用する場合、「[エンタープライズ アプリケーションの SAML トークンで発行された要求のカスタマイズ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)」を参照してください。

**要求の属性のマッピング**

1. PowerShell を使用して要求のマッピング ポリシーを構成するには、「[Customize claims emitted in tokens for a specific app in a tenant (Preview) (テナント内の特定のアプリのトークンで発行される要求をカスタマイズする (プレビュー))](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)」を参照してください。
2. ディレクトリ スキーマ拡張属性は、ユーザー オブジェクトや、グループ、テナントの詳細、サービス プリンシパルなどのその他のディレクトリ オブジェクトの追加データを Azure Active Directory に保存する方法を提供します。 アプリケーションに要求を発行するために使用できるのは、ユーザー オブジェクトの拡張属性だけです。 「[Using directory schema extension attributes in claims (要求でのディレクトリ スキーマ拡張属性の使用)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)」では、トークンの要求でアプリケーションへのユーザー データの送信にディレクトリ スキーマ拡張属性を使用する方法について説明しています。

トークンの要求に関する詳細については、以下を参照してください。

- [アクセス トークンでの要求](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Id_token での要求](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- Azure AD B2C で発行された ID トークンやアクセス トークンで想定される[要求](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims)
- [SAML トークンの要求のリファレンス](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)

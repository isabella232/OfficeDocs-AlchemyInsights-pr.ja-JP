---
title: シームレスなシングル サインオン (SSO) を構成する
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966042"
---
# <a name="configure-seamless-single-sign-on-sso"></a>シームレスなシングル サインオン (SSO) を構成する

**アプリケーションの構成**

1. アプリケーション ベンダーから値を取得する必要があります。 手動で値を入力するか、メタデータ ファイルをアップロードしてフィールドの値を抽出できます。
2. 多くのアプリは、Azure AD で動作するように事前構成されています。 これらのアプリは、Azure AD テナントにアプリを追加するときに参照できるアプリのギャラリーに一覧表示されます。 [クイックスタート シリーズ](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)では、プロセスを順を追って説明します。
3. ギャラリー以外のアプリケーションを作成するには、**[+ 独自のアプリケーションを作成]** ボタンをクリックして、アプリケーションに名前を付けます。
    - 既定では、**[ギャラリーにない他のアプリケーションを統合する]** が選択されます。これは、ギャラリー以外のアプリケーションの正しいオプションです。
    - アプリケーションの名前を入力してから **[作成]** をクリックすると、新しいギャラリー以外のエンタープライズ アプリケーションが作成されます。
    - 次に、そのアプリケーションの **[管理]** の下にある **[シングル サインオン]** に移動すると、環境に実装するためのさまざまな技法を確認できます。

**特定のアプリケーション用にシームレス SSO を構成する**

ギャラリー内のアプリについては、詳細なステップ バイ ステップの手順があります。 手順にアクセスするには、[SaaS アプリ構成チュートリアル](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)で、すべてのアプリ構成チュートリアルのリストを参照できます。

**SAML ベースの SSO を構成する**

1. [クイック スタート: Azure Active Directory (Azure AD) テナント内のアプリケーションに SAML ベースのシングル サインオン (SSO) をセットアップします](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)。
2. シングル サインオンの SAML ベースのオプションの詳細については、「[SAML ベースのシングル サインオンについて](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)」を参照してください。
3. Azure Active Directory (Azure AD) がシングル サインオン (SSO) でサポートする SAML 2.0 認証要求と応答については、「[シングル サインオンの SAML プロトコル](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)」を参照してください。
4. Azure Active Directory (Azure AD) のアプリケーション向けに、Microsoft Graph API を使用して SAML ベースのシングル サインオン (SSO) を作成して構成する方法については、「[Microsoft Graph API を使用してアプリケーション向けに SAML ベースのシングル サインオンを構成する](https://docs.microsoft.com/graph/application-saml-sso-configure-api)」を参照してください。
5. Azure AD が SAML プロトコルを使用する方法については、「[Microsoft ID プラットフォームが SAML プロトコルを使用する方法](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)」を参照してください。

**トークンと要求を構成する**

1. [方法: エンタープライズ アプリケーションの SAML トークンで発行される要求をカスタマイズします](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)。
2. PowerShell を使用して要求を構成する方法については、「[方法: テナント内の特定のアプリのトークンで発行される要求をカスタマイズする (プレビュー)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)」を参照してください。
3. オプションの要求を構成する方法については、「[方法: アプリにオプションの要求を提供する](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)」を参照してください。
4. トークンの要求でアプリケーションへのユーザー データの送信にディレクトリ スキーマ拡張属性を使用する方法については、「[要求でのディレクトリ スキーマ拡張属性の使用](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)」を参照してくだささい。
5. トークンの有効期限を構成する方法については、「[Microsoft ID プラットフォームで構成可能なトークンの有効期限 (プレビュー)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」を参照してください。
6. [トークンの有効期限ポリシーの構成 (プレビュー)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - この記事では、トークンの有効期限に新しいルールを課すのに役立つ一般的なポリシーのシナリオについて説明します。 この例では、ユーザーに Web アプリでより頻繁に認証することを要求するポリシーを作成する方法を説明します。

**SSO 構成のトラブルシューティング**

- Azure Active Directory シームレス シングル サインオン (Seamless SSO) に関するよく寄せられる質問については、「[Azure Active Directory シームレス シングル サインオン: よく寄せられる質問](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)」を参照してください。
- Azure Active Directory (Azure AD) のシームレス シングル サインオン (Seamless SSO) に関する一般的な問題について、トラブルシューティングに関する情報は、「[Azure Active Directory のシームレス シングル サインオンのトラブルシューティング](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)」を参照してください。

---
title: SSO 構成の問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7760"
- "9004346"
ms.openlocfilehash: c843e9315776f3dbab2f25c864ebe8b0c41000b8ce70046fe4eb386fce143635
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54009577"
---
# <a name="sso-configuration-issues"></a>SSO 構成の問題

1. 「[クイックスタート: アプリケーションガイドのプロパティを構成する](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)」の手順に従って、アプリケーションを構成します。
2. 選択したアプリケーションと[シングル サインオン オプション](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options)に応じて、以下の適切なガイダンスに従ってください。 a. **SAMLベースのシングルサインオン (SSO)** 用に **オンプレミス アプリケーション** を構成するには、「[アプリケーション プロキシ を使用したオンプレミスのアプリケーションに対する SAML シングル サインオン](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)」を参照してください。
    b. **パスワードベースの SSO** 用に **クラウド アプリケーション** を構成するには、「[パスワード シングル サインオンの構成](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)」を参照してください。
    c. **アプリケーション プロキシを使用したSSO** 用に **オンプレミス アプリケーション** を構成するには、「[Password vaulting for single sign-on with Application Proxy (アプリケーション プロキシを使用したシングル サインオン用のパスワード管理)](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)」を参照してください。
3. **アプリケーション プロキシの問題のトラブルシューティング**: アプリケーション プロキシ コネクタが正しく設定されているかどうかを判断するために、トラブルシューティング フロー「[Debug Application Proxy Connector issues (アプリケーション プロキシ コネクタの問題のデバッグ)](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)」の確認から始めることをお勧めします。 依然としてアプリケーションへの接続に問題がある場合は、「[Debug Application Proxy application issues (アプリケーション プロキシ アプリケーションの問題のデバッグ)](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)」に記載されているトラブルシューティング手順に従ってください。 以下のブラウザ デバッグ手順を実行し、[CORS の問題を特定](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues)できます。a. ブラウザーを起動し、Web アプリを閲覧します。
    b. **F12 キー** を押して、デバッグ コンソールを起動します。
    c. トランザクションを再現し、コンソールのメッセージを確認します。 CORS の違反により、オリジンに関するコンソール エラーが発生します。
    d.  アプリが認証のために login.microsoftonline.com にリダイレクトするときのアクセス トークンの有効期限など、一部の CORS の問題は解決できません。 アクセス トークンの有効期限が切れた結果、CORS 呼び出しは失敗します。 ユーザーのセッション中にアクセス トークンの有効期限が切れないようにアクセス トークンの有効期限を延長することが、このシナリオの回避策です。 これを行う方法の詳細については、「[Configurable token lifetimes in Microsoft identity platform (Microsoft ID プラットフォームで構成可能なトークンの有効期限)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」を参照してください。
4. **SAML ベースの SSO のトラブルシューティング**: 「[SAML ベースのシングル サインオンで構成されたアプリへのサインインに関する問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)」をチェックして、発生する可能性が最も高い問題の解決策を見つけることをお勧めします。
5. **パスワード ベースの SSO のトラブルシューティング**: 「[Azure AD でのパスワード ベースのシングル サインオンのトラブルシューティング](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)」をチェックして、発生する可能性が最も高い問題の解決策を見つけることをお勧めします。
6. **構成エラーを受け取りました**: 構成エラーのトラブルシューティングを行うには、次の記事を確認することをお勧めします。a. 「[SAML ベースのシングル サインオンで構成されたアプリへのサインインに関する問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)」 b. 「[資格情報を入力したが、拡張機能によって送信されない](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso#credentials-are-filled-in-but-the-extension-does-not-submit-them)」 c. 「[資格情報を入力して送信したが、ページには資格情報が正しくないと表示される](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)」d. 「[ユーザーのサインイン後、アプリのページでエラーが発生する](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)」
7. **シームレス SSO とオンプレミス アプリの統合に問題があります**: シームレス SSO とオンプレミス アプリの統合に関する問題のトラブルシューティングを行うには、次の記事を確認することをお勧めします。 「[ アプリケーション プロキシ アプリケーションへのシングル サインオンの構成方法](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)」b. 「[アプリケーション プロキシを使用したオンプレミス アプリケーションの SAML シングル サインオン](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)」c. 「[Azure Active Directory アプリケーション プロキシの CORS の問題を理解し、解決する](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)」d. 「[アプリケーション プロキシの Kerberos の制約付き委任構成のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)」
8. **要求を修正するか、トークンの有効期間を延長する必要があります。 セッションの長さを変更する必要があります**: これを行うには、次の記事を確認することをお勧めします。a. 「[アプリケーションに送信される SAML 要求をカスタマイズする](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)」b. 「[要求対応アプリの操作](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications)」c. 「[Microsoft ID プラットフォームで構成可能なトークンの有効期間](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」d. 「[条件付きアクセスを使用して認証セッション管理を構成する](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime)」e. 「[オンプレミスのアプリケーションにアクセスするための Cookie 設定](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings)」
9. **ユーザーおよびゲスト ユーザー (B2B) のアクセスの管理についてサポートが必要です**: ユーザーおよびゲストユーザーのアクセスの管理の詳細については、次の記事を確認することをお勧めします。a. 「[アプリへのアクセスの管理](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-access-management)」b. 「[Azure Active Directory のアプリに対するユーザー割り当ての管理](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)」c. 「[B2B コラボレーション用の SaaS アプリの構成](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)」d. 「[Azure AD の B2B ユーザーにオンプレミスのアプリケーションへのアクセスを許可する](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)」e. 「[Azure AD B2B コラボレーションを使用して、ローカルで管理されているパートナー アカウントにクラウド リソースへのアクセスを許可する](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)」
10. **アプリをカスタマイズしたい**: アプリのカスタマイズの詳細については、次の記事を確認することをお勧めします。a. 「[Azure AD アプリケーション プロキシでカスタム ドメインを構成する](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain)」b. 「[発行されたアプリのカスタム ホーム ページを設定する](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-home-page)」c. 「[ワイルドカード アプリケーション](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard)」
11. **AD FS から Azure へのアプリの移行で問題が発生しました**: AD FS から Azure へのアプリの移行中に発生した問題のトラブルシューティングを行うには、次の記事を確認することをお勧めします。a. 「[アプリケーション認証を Active Directory フェデレーション サービス (AD FS) から Azure Active Directory に移動する](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-apps-to-azure)」b. 「[アプリケーションを Azure Active Directory に移行するためのリソース](https://docs.microsoft.com/azure/active-directory/manage-apps/migration-resources)」


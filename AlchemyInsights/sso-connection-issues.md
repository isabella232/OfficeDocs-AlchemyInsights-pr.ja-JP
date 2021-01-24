---
title: SSO 接続に関する問題
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
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935226"
---
# <a name="sso-connection-issues"></a>SSO 接続に関する問題

1. 「[クイックスタート: アプリケーションガイドのプロパティを構成する](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)」の手順に従って、アプリケーションを構成します。
2. 選択したアプリケーションと[シングル サインオン オプション](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options)に応じて、以下の適切なガイダンスに従ってください。
    - **SAMLベースのシングル サインオン** 用に **オンプレミス アプリケーション** を構成するには、「[アプリケーション プロキシ を使用したオンプレミスのアプリケーションに対する SAML シングル サインオン](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)」を参照してください。
    - **パスワードベースのシングル サインオン** 用に **クラウド アプリケーション** を構成するには、「[パスワード シングル サインオンの構成](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)」を参照してください。
    - **アプリケーション プロキシを使用したシングル サインオン** 用に **オンプレミス アプリケーション** を構成するには、「[アプリケーション プロキシを使用したシングル サインオン用のパスワード管理](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)」を参照してください。
3. **アプリケーション プロキシの問題のトラブルシューティング**: アプリケーション プロキシ コネクタが正しく設定されているかどうかを判断するために、トラブルシューティング フロー「[アプリケーション プロキシ コネクタの問題のデバッグ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)」の確認から始めることをお勧めします。 依然としてアプリケーションへの接続に問題がある場合は、「[アプリケーション プロキシ アプリケーションの問題のデバッグ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)」に記載されているトラブルシューティング フローに従ってください。 ブラウザ デバッグ ツールを使用し、[CORS の問題を特定](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues)できます。
    - ブラウザーを起動し、Web アプリを閲覧します。
    - **F12 キー** を押して、デバッグ コンソールを起動します。
    - トランザクションを再現し、コンソールのメッセージを確認します。 CORS の違反により、オリジンに関するコンソール エラーが発生します。
    - CORS の問題の一部は、アプリが認証のために login.microsoft.com にリダイレクトされたり、アクセス トークンが期限切れになったりする場合など、解決できない場合があります。 その後、CORS の呼び出しは失敗します。 ユーザーのセッション中にアクセス トークンの有効期限が切れないようにアクセス トークンの有効期限を延長することが、このシナリオの回避策です。 これを行う方法の詳細については、「[Configurable token lifetimes in Microsoft identity platform (Microsoft ID プラットフォームで構成可能なトークンの有効期限)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」を参照してください。
4. **SAML ベースのシングル サインオンのトラブルシューティング**: 「[SAML ベースのシングル サインオンで構成されたアプリへのサインインに関する問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)」をチェックして、発生する可能性が最も高い問題の解決策を見つけることをお勧めします。
5. **パスワード ベースのシングル サインオンのトラブルシューティング**: 「[Azure AD でのパスワード ベースのシングル サインオンのトラブルシューティング](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)」をチェックして、発生する可能性が最も高い問題の解決策を見つけることをお勧めします。
6. VPN 使用中の接続に関する問題については、「[VPN および Wi-Fi 接続でシングル サインオン (SSO) を使用する方法](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)」を参照してください。

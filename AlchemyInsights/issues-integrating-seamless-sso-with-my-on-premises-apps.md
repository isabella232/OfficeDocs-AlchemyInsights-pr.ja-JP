---
title: 自分のオンプレミス アプリとシームレスな SSO の統合に関する問題
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028297"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>自分のオンプレミス アプリとシームレスな SSO の統合に関する問題

オンプレミス アプリケーションとのシームレスな SSO の統合に関する問題をトラブルシューティングするには、次の操作を行います。

**推奨される手順**

1. **アプリケーション プロキシを使用したシングル サインオン** 用に **オンプレミス アプリケーション** を構成するには、「[Password vaulting for single sign-on with Application Proxy (アプリケーション プロキシを使用したシングル サインオン用のパスワード管理)](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)」を参照してください。
1. **アプリケーション プロキシの問題のトラブルシューティング**: アプリケーション プロキシ コネクタが正しく設定されているかどうかを判断するために、トラブルシューティング フロー「[Debug Application Proxy Connector issues (アプリケーション プロキシ コネクタの問題のデバッグ)](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)」の確認から始めることをお勧めします。 依然としてアプリケーションへの接続に問題がある場合は、「[Debug Application Proxy application issues (アプリケーション プロキシ アプリケーションの問題のデバッグ)](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)」に記載されているトラブルシューティング手順に従ってください。 以下のブラウザ デバッグ ツールを使用し、[CORS の問題を特定](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues)できます。
    1. ブラウザーを起動し、Web アプリを閲覧します。
    1. **F12 キー** を押して、デバッグ コンソールを起動します。
    1. トランザクションを再現し、コンソールのメッセージを確認します。 CORS の違反により、オリジンに関するコンソール エラーが発生します。
    1. CORS の問題の一部は、アプリが認証のために login.microsoftonline.com にリダイレクトされたり、アクセス トークンが期限切れになったりする場合など、解決できない場合があります。 その後、CORS の呼び出しは失敗します。 ユーザーのセッション中にアクセス トークンの有効期限が切れないようにアクセス トークンの有効期限を延長することが、このシナリオの回避策です。 これを行う方法の詳細については、「[Configurable token lifetimes in Microsoft identity platform (Microsoft ID プラットフォームで構成可能なトークンの有効期限)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」を参照してください。

**おすすめのドキュメント**

- [ アプリケーション プロキシ アプリケーションへのシングル サインオンの構成方法](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [アプリケーション プロキシを使用したオンプレミス アプリケーションの SAML シングル サインオン](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Azure Active Directory アプリケーション プロキシの CORS の問題を理解し、解決する](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [アプリケーション プロキシの Kerberos の制約付き委任構成のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
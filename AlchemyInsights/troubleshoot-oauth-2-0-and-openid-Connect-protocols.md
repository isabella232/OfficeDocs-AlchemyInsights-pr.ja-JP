---
title: OAuth 2.0 および OpenID Connect プロトコルのトラブルシューティング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038316"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>OAuth 2.0 および OpenID Connect プロトコルのトラブルシューティング

OAuth 2.0 と OpenID Connect の問題を解決するには、次の推奨手順を実行します。

OAuth 2.0 および OpenID Connect プロトコルの構成とトラブルシューティングに関連する次の記事を参照してください。

- [Microsoft ID プラットフォームおよび OAuth 2.0 認証コードのフロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow): - この記事は、任意の言語を使用して、アプリケーションの **コード付与 (PKCE) フロー** に対して直接プログラミングする方法について説明しています。
- [Microsoft ID プラットフォームおよび OAuth 2.0 クライアント資格情報フロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow): この記事は、アプリケーション内の **クライアント資格情報フロー** に対して直接プログラムする方法を説明しています。
- [Microsoft ID プラットフォームと OAuth 2.0 リソース所有者パスワード資格情報](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - この記事では、アプリケーション内の **ROPC フロー** に対して直接プログラムを実行する方法について説明します。
    - Microsoft ID プラットフォームは Azure AD テナント向けの ROPC のみサポートし、個人アカウントはサポートしていません。 つまり、テナント固有のエンドポイント アプリケーション **(https://login.microsoftonline.com/{TenantId_or_Name})** または **組織** エンドポイントを使用する必要があります。
    - Azure AD テナントに招待されている個人アカウントは、ROPC を使用できません。
    - パスワードのないアカウントは、ROPC からサインインできません。 このシナリオでは、代わりに別のフローをアプリに使用することをお勧めします。
    - ユーザーがアプリケーションへのログインに[多要素認証 (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) を使用する必要がある場合、ブロックされます。
    - ROPC は、[ハイブリッド ID フェデレーション シナリオ](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (オンプレミス アカウントの認証に使用される Azure AD と ADFS など) ではサポートされていません。 ユーザーがオンプレミスの ID プロバイダーにフル ページでリダイレクトされる場合、Azure AD は、その ID プロバイダーに対してユーザー名とパスワードをテストできません。 ただし、[パススルー認証](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta)は ROPC でサポートされています。
    - ハイブリッド ID フェデレーションのシナリオの例外には、次のようなシナリオがあります。 **AllowCloudPasswordValidation** が **TRUE** に設定されたホーム領域検出ポリシーにより、オンプレミスのパスワードがクラウドに同期されたときに、ROPC フローがフェデレーション ユーザーに対して有効になる。 詳細については、「[レガシ アプリケーションのフェデレーション ユーザーの直接 ROPC 認証を有効にする](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications)」を参照してください。 
- [Microsoft ID プラットフォームと OAuth 2.0 の代理フロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) - この記事では、アプリケーションの **代理 (OBO) フロー** に対して、直接プログラムを実行する方法について説明します。
- [Microsoft ID プラットフォームおよび OpenID Connect プロトコル](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc): この記事は、言語に依存しない Open ID Connect プロトコルを実装する方法と、Microsoft オープンソース ライブラリを使用せずに HTTP メッセージを送受信する方法について説明します。

**アクセス トークン**

[Microsoft ID プラットフォームのアクセス トークン](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - API がアクセス トークン内のクレームを検証および使用する方法について説明します。 特に明示されている場合を除き、この記事のすべてのドキュメントは、登録した API に対して発行されるトークンにのみ適用されます。 これは、Microsoft 所有の API で発行されるトークンには適用されません。また、これらのトークンを使用して、作成した API に対して Microsoft ID プラットフォームがトークンを発行する方法を検証することもできません。

**アプリケーション構成**

[リダイレクト URI (返信 URL) の制限事項](https://docs.microsoft.com/azure/active-directory/develop/reply-url) - リダイレクト URI (返信 URL) を構成する方法について説明します。 リダイレクト URI (返信 URL) とは、アプリが正常に承認され、認証コードまたはアクセス トークンが付与された後に、承認サーバーがユーザーを送る場所です。 承認サーバーがコードまたはトークンをリダイレクト URI に送信します。そのため、アプリの登録プロセスの一環として、正しい場所を登録することが重要です。

**アプリケーションのプロビジョニング**

[チュートリアル: SCIM エンドポイントのプロビジョニングを開発および計画する](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) - この記事では、SCIM エンドポイントを構築し、AAD プロビジョニング サービスと統合する方法について説明します。



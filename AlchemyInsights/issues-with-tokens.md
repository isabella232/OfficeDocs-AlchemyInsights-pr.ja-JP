---
title: トークンに関する問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917280"
---
# <a name="issues-with-tokens"></a>トークンに関する問題

トークンに関する問題を管理するには、次の手順を実行します。

1. Microsoft ID プラットフォームによって発行されるアクセス、ID、または SAML トークンの有効期限を指定できます。 組織のすべてのアプリ、マルチテナント (多組織) アプリケーション、組織の特定のサービス プリンシパルにトークンの有効期間を設定できます。 詳細については、「[Microsoft ID プラットフォームで構成可能なトークンの有効期限 (プレビュー)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」を参照してください。
2. アクセス トークンを使用すると、クライアントは保護された Web API を安全に呼び出すことができ、Web API は認証および認可を実行するために使用します。 OAuth 仕様によると、アクセス トークンは、設定された形式を持たない不透明な文字列です。ID プロバイダー (IDP) によっては、GUID を使用するものもあれば、暗号化された BLOB を使用するものもあります。 Microsoft ID プラットフォームでは、トークンを受け入れる API の構成に応じて、さまざまなアクセス トークン形式が使用されます。 API がアクセス トークン内のクレームを検証および使用する方法については、「[Microsoft ID プラットフォームのアクセス トークン](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint)」を参照してください。
3. Microsoft Authentication Library (MSAL) は、さまざまなアプリケーション シナリオで使用する複数の認証フローをサポートします。 詳細については、「[認証フロー](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes)」を参照してください。
4. OAuth 2.0 認証コード付与は、デバイスにインストールされているアプリで、Web API などの保護されたリソースにアクセスするために使用できます。 OAuth 2.0 の Microsoft ID プラットフォームの実装を使用すると、モバイル アプリおよびデスクトップ アプリにサインインおよび API アクセスを追加できます。 任意の言語を使用して、アプリケーションのプロトコルに対して直接プログラミングする方法については、「[Microsoft ID プラットフォームおよび OAuth 2.0 認証コードのフロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token)」を参照してください。
5. OpenID Connect (OIDC) は、OAuth 2.0 上に構築された認証プロトコルで、ユーザーをアプリケーションに安全にサインインするために使用できます。 Microsoft ID プラットフォーム エンドポイントの OpenID Connect の実装を使用する場合、アプリにサインインと API アクセスを追加できます。 [Microsoft ID プラットフォームおよび OpenID Connect プロトコル](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request)は、言語に依存せずに実行する方法を示し、Microsoft オープンソース ライブラリを使用せずに HTTP メッセージを送受信する方法を説明します。
    - UserInfo エンドポイントは OIDC 標準の一部であり、認証されたユーザーに関する要求を返すように設計されています。 詳細については、「[Microsoft ID プラットフォームの UserInfo エンドポイント](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead)」を参照してください。
    - [Azure AD と OpenID Connect を使用した Web アプリの Web API の呼び出し](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/)サンプルは、OpenID Connect プロトコルを使用して Azure AD でサインインする MVC Web アプリケーションを作成し、OAuth 2.0 経由で入手したトークンを使用してサインインしたユーザーの ID で Web API を呼び出す方法を示します。 このサンプルは、OpenID Connect ASP .Net OWIN ミドルウェアと ADAL .Net を使用します。
6. [アプリケーションで Web API を公開するように構成する](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) - このクイックスタートでは、Microsoft ID プラットフォームに Web API を登録し、サンプル範囲を追加してクライアント アプリに公開します。 Web API を登録し、範囲を介して公開することにより、認証されたユーザーおよび API にアクセスするクライアント アプリに対してリソースへのアクセス許可ベースのアクセスを提供できます。
7. Azure Active Directory B2C (Azure AD B2C) では、リソース所有者パスワード資格情報 (ROPC) フローは OAuth 標準認証フローです。 このフローでは、アプリケーション (証明書利用者とも呼ばれる) がトークンの有効な資格情報を交換します。 資格情報には、ユーザー ID とパスワードが含まれます。 返されるトークンは、ID トークン、アクセス トークン、および更新トークンです。 詳細については、「[Azure Active Directory B2C でリソース所有者のパスワード資格情報フローをセットアップする](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow)」を参照してください。 


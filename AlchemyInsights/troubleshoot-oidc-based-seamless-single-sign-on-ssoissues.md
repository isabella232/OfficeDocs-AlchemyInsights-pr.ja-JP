---
title: OIDC ベースのシームレス シングル サインオン (SSO) の問題のトラブルシューティング
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
- "9004357"
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105783"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>OIDC ベースのシームレス シングル サインオン (SSO) の問題のトラブルシューティング

- Azure テナントに OIDC ベースのアプリを追加する方法については、「 [クイック スタート: Azure Active Directory (Azure AD) テナント内のアプリケーションに OIDC ベースのシングル サインオン (SSO) をセットアップする](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)」を参照してください。
- OpenID 接続の標準を使用してシングル サインオンを実装するアプリの詳細については、「[OIDC ベースのシングル サインオンを理解する](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)」を参照してください。
- Microsoft のオープン ソース ライブラリを使用せずに、HTTP 要求を直接送信して処理したり、サードパーティのオープン ソース ライブラリを使用してコードを作成する場合の詳細については、「[Microsoft ID プラットフォームの OAuth 2.0 および OpenID Connect プロトコル](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)」を参照してください。

**プロトコル**

1. [Microsoft ID プラットフォームと暗黙の許可フロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) - 暗黙の許可の明確な特徴としては、トークン (ID トークンまたはアクセス トークン) が/token エンドポイントではなく/承認エンドポイントから直接返されるという点があります。 これは多くの場合、 **"ハイブリッド フロー" と呼ばれる認証コード フローの一部として使用されます。認証コードと共に/承認要求で ID トークンを取得します**。 この記事では、Azure AD からトークンを要求するために、アプリケーション内のプロトコルに対して直接プログラムを実行する方法について説明します。
2. [Microsoft ID プラットフォームと OAuth 2.0 認証コード フロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - OAuth 2.0 承認コードの付与は、Web API などの保護されたリソースにアクセスするために、デバイスにインストールされているアプリで使用できます。 OAuth 2.0 の Microsoft ID プラットフォームの実装を使用すると、**モバイル アプリおよびデスクトップ アプリにサイン インおよび API アクセスを追加** できます。 この記事では、任意の言語を使用して、アプリケーションのプロトコルに対して直接プログラムを実行する方法について説明します。
3. [Microsoft ID プラットフォームと OpenID 接続プロトコル](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Microsoft ID プラットフォームで実装されている OpenID 接続を使用する場合、アプリにサインインと API アクセスを追加できます。 この記事では、言語に依存せずに実行する方法を示し、**Microsoft オープンソース ライブラリを使用せずに HTTP メッセージを送受信する** 方法を説明します。
4. [Microsoft ID プラットフォームと OAuth 2.0 クライアントの資格情報フロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - RFC 6749 で指定された OAuth 2.0 クライアント資格情報付与 (**2 本足の OAuth** と呼ばれることもある)を使用して、アプリケーションの ID を使って Web でホストされるリソースにアクセスすることができます。 この種の付与は、ユーザーとすぐに対話することなく、バックグラウンドで実行する必要があるサーバー間の対話で一般的に使用されます。 これらの種類のアプリケーションは、多くの場合、**デーモン** または **サービス アカウント** と呼ばれます。 この記事では、アプリケーション内のプロトコルに対して直接プログラムを実行する方法について説明します。

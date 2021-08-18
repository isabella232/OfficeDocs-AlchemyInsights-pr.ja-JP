---
title: リンクおよび URL に関する問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: d85069970fe6bc6cc7a8488c49c0e6236426d45b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321912"
---
# <a name="issues-with-links-and-urls"></a>リンクおよび URL に関する問題

リダイレクト URI/応答 URL (どちらの表現も置き替え可能) は、Microsoft ID プラットフォームがアプリ要求トークンを返すために使用する URL です。これらの URL の詳細については、以下の記事を参照してください。

- [認証フローとアプリケーション シナリオ](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - 各シナリオの **アプリ登録** ページのリダイレクト URI に関する情報。
- [リダイレクト URI/応答 URL の制限事項](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**アプリの正しいリダイレクト URI/応答 URL の登録方法がわかりません**

開発中のアプリケーションでサインインするときに、サインイン ダイアログに **AADSTS50011 と表示される場合: 要求で指定された応答 URL がアプリケーション <your app ID>** に構成された応答 URL と一致しません。アプリケーション登録に、Microsoft ID プラットフォームへのトークン要求で使用したコードのリダイレクト URI を追加する必要があります。

応答 URL を追加するには、Azure portal の **アプリケーション登録** ページの **[認証]** タブに移動し、**リダイレクト URI** セクションにエントリを追加します。 入力する必要がある値は、次に説明するように、作成するアプリケーションの種類によって異なります。

- シングルページ アプリケーションおよび Web アプリの場合、応答 URL はアプリケーション内の URL です。 「[シングルページのアプリケーション登録](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri)」または「[Azure portal を使用した Web アプリの登録](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)」を参照
- デスクトップ アプリの場合、選択する必要がある値は次の条件によって異なります。
    - プラットフォーム (MacOS は Windows または Linux とは異なる)
    - トークンの取得方法 (対話型でデバイス コード フロー、統合 Windows 認証 [IWA]、またはユーザー名/パスワードを使用)
    詳細については、「[デスクトップ アプリ - アプリ登録 - リダイレクト URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)」を参照してください。
- モバイル アプリケーションの場合、リダイレクト URI は次の条件によって異なります。
    - プラットフォーム (iOS/Android/UWP)
    - iOS のバンドル ID、Android のパッケージ名と署名ハッシュなど、アプリを作成するために使用される情報 Azure portal アプリの登録が役立ちます。 詳細については、「[プラットフォーム構成およびリダイレクト URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)」を参照してください。

**注**: Web API およびトークン取得の一部のサイレント方法 (IWA およびユーザー名/パスワード) には、リダイレクト URI は必要ありません。

**Web アプリケーションを展開しましたが、展開したアプリをテストすると URL 不一致メッセージが表示されます**

Web アプリケーションを展開しているすべてのロケーションにリダイレクト URI を追加します。 詳細については、「[Azure portal を使用して Web アプリを登録する](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)」を参照してください。

**注**: アプリケーションをロケーションに展開した直後に、そのロケーションのリダイレクト URI を追加します。

**応答 URL を十分に登録できません**

ISV であり、お客様ごとに 1 つまたは複数のリダイレクト URI があります。 ADAL/Azure AD v1.0 から MSAL/Microsoft ID プラットフォームに移行する場合、[リダイレクト URI の最大数](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)に達します。 これを解決するには、お客様ごとに対応する[サービス プリンシパルにリダイレクト URI を追加](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals)します。

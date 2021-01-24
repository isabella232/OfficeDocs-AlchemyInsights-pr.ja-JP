---
title: シームレス SSO のユーザー サインインに関する問題
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
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935228"
---
# <a name="seamless-sso-user-sign-in-issues"></a>シームレス SSO のユーザー サインインに関する問題

ユーザーが認証されると、ブラウザーはユーザーの認証情報をキャッシュし、アプリケーションが同じブラウザーで同じアカウントを使用して自動的にサインインするようにします。 これにより、別のユーザーまたは単一のユーザーが 1 つのデバイスで複数のアカウントにログインするのが難しいことがあります。 この問題を解決するには、次の手順を実行します。1. 別のブラウザーでサインインします。 2. ブラウザーのキャッシュとクッキーを消去し、もう一度サインインします。

サインインに関する問題が引き続き発生する場合、診断と解決手順を自動化するために次のことをお勧めします。

1. [My Apps Secure Browser Extension](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) をインストールします。これをインストールすると、Azure portal でテスト体験を使用するとき、Azure Active Directory (Azure AD) からより良い診断と解決策が得られます。
2. Azure portal のアプリ構成ページにあるテスト体験を使用し、エラーを再現します。 詳細については、[SAML ベースのシングル サインオン アプリケーションをデバッグする](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)方法に関するページを参照してください。
3. My Apps Secure Browser Extension を使用して、Azure portal でテスト体験を使用する場合は、**手順 4 を省略** できます。
4. [SAML ベースのシングル サインオンの構成] ページを開くには、次の手順を行います。
    - [Azure portal](https://portal.azure.com/) を開き、**グローバル管理者**、または **共同管理者** としてサインインします。
    - 左側のメイン ナビゲーション メニューの上部にある **[すべてのサービス]** を選択して **[Azure Active Directory 拡張機能]** を開きます。
    - フィルター検索ボックスに "Azure Active Directory" と入力し、**[Azure Active Directory]** 項目を選択します。
    - Azure Active Directory の左側のナビゲーション メニューから **[エンタープライズ アプリケーション]** を選択します。
    - **[すべてのアプリケーション]** を選択して、すべてのアプリケーションの一覧を表示します。 ここに表示したいアプリケーションが表示されない場合は、**[All Applications List (すべてのアプリケーション リスト)]** の上部にある **[フィルター]** コントロールを使用して、**[表示]** オプションを **[すべてのアプリケーション]** に設定します。
    - シングル サインオンを構成するアプリケーションを選択します。
    - アプリケーションが読み込まれた後、アプリケーションの左側にあるナビゲーション メニューで **[シングル サインオン]** をクリックします。
    - **[SAML ベースの SSO]** を選択します。
5. エラーに基づいて推奨される次の手順の詳細については、「[SAML ベースのシングル サインオンで構成されたアプリへのサインインに関する問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)」を参照してください。
6. その他のユーザー サインに関する問題のトラブルシューティングを行うには、次のガイダンスを参照してください。
    - [シングル サインオンの SAML プロトコル](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [方法: Azure Active Directory レポートを使用してサインイン エラーをトラブルシューティングする](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [予期しない同意プロンプト](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [ユーザーの同意エラー](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [マイ アプリからのサインインに関する問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [アプリケーションのサインイン ページでのエラー](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Microsoft アプリへのサインインに関する問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)

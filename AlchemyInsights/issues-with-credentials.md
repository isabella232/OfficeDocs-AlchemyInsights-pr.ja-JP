---
title: 資格情報に関する問題
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063734"
---
# <a name="issues-with-credentials"></a>資格情報に関する問題

[Microsoft ID プラットフォームおよび OAuth 2.0 クライアント資格情報フロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)は、OAuth 2.0 クライアント資格情報付与フローに対して直接プログラムする方法を説明しています。

**アプリケーションのパスワードまたは証明書の資格情報を管理するする方法**

Azure CLI では、[az ad app 資格情報](https://docs.microsoft.com/cli/azure/ad/app/credential)を使用して、アプリケーションのパスワードまたは証明書の資格情報を削除、一覧表示、またはリセットできます。

**ユーザーがパスワードをリセットする方法**

ユーザーは、パスワードをリセットする前に、[セルフサービスによるパスワードのリセットに登録する](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register)必要があります。 ユーザーが登録すると、この記事の手順に従ってパスワードをリセットできます: [職場または学校のパスワードをリセットする](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**ユーザーがパスワードを変更する方法**

ユーザーは、この記事の手順に従ってパスワードを変更できます: [パスワードを変更する方法](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
また、[2 段階認証のためにアプリ パスワードを管理する](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)こともできます。

**パスワードを変更またはリセットすると、ユーザーにエラーが発生します**

このリンクは、ユーザーがパスワードをリセットしようとしたときに発生する一般的な問題に関する情報を提供します: [一般的な問題とその解決策](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**ユーザーのパスワードのリセット中に問題が発生しました**

- パスワードをリセットする権限があることを確認します。 *グローバル、パスワード、およびユーザー管理者のみがユーザー パスワードをリセットできます。* グローバル管理者は、他の特権を持つ管理者のパスワードをリセットすることもできます。

- ライセンス要件を理解していることを確認します。

  - 組織内で少なくとも 1 つのライセンスが割り当てられている必要があります。
    - **クラウド専用ユーザー** - 任意の Office 365 (O365) 有料 SKU または Azure AD Basic
    - **クラウドとオンプレミス ユーザー** - Azure AD Premium P1 または P2、Enterprise Mobility + Security (EMS)、または Secure Productive Enterprise (SPE)
    - ライセンス要件の詳細については、「[Azure AD セルフサービスによるパスワードのリセットのライセンス要件](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)」を参照してください。
- ユーザーのパスワードをリセットするには、Azure AD でユーザーを検索します。 次に、そのユーザーの概要ブレードで、[パスワードのリセット] ボタンをクリックします。

**[パスワードのリセット] ボタンが灰色表示されています**

**この** ユーザーのパスワードをリセットする権限がありません。 *グローバル、パスワード、およびユーザー管理者のみがユーザー パスワードをリセットできます。* グローバル管理者は、他の特権を持つ管理者のパスワードをリセットすることもできます。

**パスワード リセット ブレードが表示されていません**

パスワードをリセットする権限がありません。 *グローバル、パスワード、およびユーザー管理者のみがユーザー パスワードをリセットできます。* グローバル管理者は、他の特権を持つ管理者のパスワードをリセットすることもできます。

**[パスワードのリセット] にオンプレミス統合ブレードが表示されていません**

- オンプレミス統合ブレードは、ハイブリッド環境だけで表示されます。つまり、パスワードの書き戻しを使用してオンプレミス ユーザーのパスワードを操作します。

- 次の場合、このブレードは表示されません。

  - パスワードの書き戻しを使用していない
  - パスワードの書き戻しのインストール/接続に問題がある
  - Azure AD Connect のインストール/接続に問題がある
  - パスワードの書き戻しに関する問題のトラブルシューティングの手順については、「[パスワードの書き戻しに関するトラブルシューティング](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)」を参照してください。

**ユーザーのパスワードをリセットする方法がわかりません**

1. パスワードをリセットできる適切な管理者として Azure portal にサインインします。
2. **[ユーザーおよびグループ]** ブレードに移動し、**[すべてのユーザー]** を選択します。
3. 一覧からユーザーを選択します。
4. 選択したユーザーに対して、**[概要]** を選択し、コマンド バーで **[パスワードのリセット]** を選択します。
5. **[パスワードのリセット]** ボタンを選択し、画面の指示に従います。
    - **Azure portal** で実行されるリセットのみ、パスワードの書き戻しをサポートします。

**Office 365 管理ポータルまたは Office 365 モバイル アプリケーションからオンプレミス ユーザーのパスワードをリセットしましたが、ユーザーがまだサインインできません**

このポータルでは、パスワードの書き戻しはサポートされていません。 Azure portal でユーザーのパスワードをリセットします。

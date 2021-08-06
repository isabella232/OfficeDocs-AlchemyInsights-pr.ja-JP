---
title: パスワードの書き戻しが機能しません
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
- "9004595"
- "8210"
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999749"
---
# <a name="password-writeback-is-not-working"></a>パスワードの書き戻しが機能しません

**パスワードの書き戻しの設定に問題があります**

- パスワードの書き戻しはプレミアム機能です。
- ライセンス要件を理解していることを確認します。
  - 組織内で少なくとも 1 つのライセンスが割り当てられている必要があります。
  - **クラウド専用ユーザー** - 任意の Office 365 (O365) 有料 SKU または Azure AD Basic
  - **クラウドとオンプレミス ユーザー** - Azure AD Premium P1 または P2、Enterprise Mobility + Security (EMS)、または Secure Productive Enterprise (SPE)
    - ライセンス要件の詳細については、「[Azure AD セルフサービスによるパスワードのリセットのライセンス要件](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)」を参照してください。
- 適切なライセンスの 1 つを持つ、少なくとも 1 つの管理者アカウントと 1 つのテスト ユーザー アカウントがあります。
- パスワードの書き戻しを機能させるには、Azure AD Connect をプライマリ ドメイン コントローラーのエミュレーターに接続する必要があります。 Active Directory 同期コネクタの **[プロパティ]** を右クリックし、**[ディレクトリ パーティションを構成する]** を選択することで、プライマリ ドメイン コントローラーを使用するように Azure AD Connect を構成できます。 そこから、**[ドメイン コントローラーの接続設定]** セクションを探し、**[優先ドメイン コントローラーのみを使用する]** というタイトルのチェック ボックスをオンにします。
  > [!NOTE]
  > 優先 DC が PDC エミュレーターでない場合でも、Azure AD Connect はパスワードの書き戻しのために PDC に連絡します。
- テナントでパスワードのリセットが構成され、有効になっています。 詳細については、「[ユーザーが Azure AD パスワードをリセットできるようにする](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)」をご覧ください。
- パスワードの書き戻しを有効にするために使用されている管理者アカウントがクラウド管理者アカウントであることを確認してください (オンプレミス AD ではなく Azure AD で作成されます)
- Windows Server 2008 R2、Windows Server 2012、または最新のサービスパックがインストールされた Windows Server 2012 R2 を実行しているシングルまたはマルチフォレスト AD オンプレミス展開があります
- Azure AD Connect ツールがインストールされており、クラウドと同期するための AD 環境が準備されています。 パスワードの書き戻しをテストする前に、Azure AD Connect で AD と Azure AD の両方から完全なインポートと完全な同期を完了していることを最初に確認してください。
- 詳細については、「[Azure AD Connect での完全同期と完全インポート](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)」をご覧ください。

**パスワードの書き戻し接続に問題があります**

1. 最新バージョンの [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594) をダウンロードして有効にします
2. ファイアウォール構成: Azure AD Connect ツール (1.1.443 以降) には、以下への **アウトバウンド HTTPS** アクセスが必要です。
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. アイドル状態の接続を、少なくとも 2-3 分間持続させます

**パスワードの書き戻しにまだ問題があります**

- それでも問題が解決しない場合は、Azure AD Connect ツールで パスワードの書き戻しサービスを無効にしてから再度有効にしてみてください
- 詳細については、[パスワードの書き戻しを無効にしてから再度有効にする](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)方法をご覧ください。

---
title: パスワードのリセットに関する問題
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039971"
---
# <a name="problems-resetting-password"></a>パスワードのリセットに関する問題

パスワードをリセットするときに発生する可能性がある問題と、考えられる解決策を次に示します。

**他のカテゴリで取り上げられていない、パスワードのリセットに関する問題が発生する**

- パスワードをリセットする権限があることを確認します。 グローバル管理者、パスワード管理者、およびユーザー管理者のみがユーザー パスワードをリセットできます。 グローバル管理者は、他の特権を持つ管理者のパスワードをリセットすることもできます。
- ライセンス要件を理解していることを確認します。
    - 組織内で少なくとも 1 つのライセンスが割り当てられている必要があります。
        - クラウド専用ユーザー - 任意の Office 365 (O365) 有料 SKU または Azure AD Basic
        - クラウドとオンプレミス ユーザー - Azure AD Premium P1 または P2、Enterprise Mobility + Security (EMS)、または Secure Productive Enterprise (SPE)
        - ライセンス要件の詳細については、「[Azure AD セルフサービスによるパスワードのリセットのライセンス要件](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)」の記事を参照してください。

**設定したパスワード リセット ポリシーのテストで問題が発生している**

- 最近適用したポリシーは、すべてのデータ センターとエンド ポイント間で複製するため、数分かかる場合があります。 データ センターからの物理的な距離も、変更が適用されるスピードに影響します。
- 管理者ではなくエンド ユーザーとテストし、小さなユーザーの一群をパイロットします。 Azure ポータルで構成されたポリシーはエンドユーザーにのみ適用され、管理者には適用されません。 Microsoft は、Azure 管理者ロールに強力な既定の 2 段階パスワード リセット ポリシーを適用しています (例: グローバル管理者、ヘルプデスク管理者、パスワード管理者など)。
    - 「[管理者のポリシー](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)」の詳細については、次をご覧ください。

**パスワードのリセットを展開したいが、ユーザーに追加のセキュリティ情報の登録を許可したくない**

ユーザーのために事前入力されているため、ユーザーが入力する必要はありません。 - 管理者は、組織にパスワードのリセットを展開する前に、ユーザーの電話とメールのプロパティを設定できます。 これは、API、PowerShell、または Azure AD Connect を使用して行うことができます。 詳細情報については、こちらを参照してください。
- [ユーザーに登録を求めることなくパスワードのリセットを展開する](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [パスワードのリセットで使用されるデータ](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**[パスワードのリセット] ボタンが灰色表示されています**

このユーザーのパスワードをリセットする権限がありません。 グローバル管理者、パスワード管理者、およびユーザー管理者のみがユーザー パスワードをリセットできます。 グローバル管理者は、他の特権を持つ管理者のパスワードをリセットすることもできます。

**パスワード リセット ブレードが表示されていません**

パスワードをリセットする権限がありません。 グローバル管理者、パスワード管理者、およびユーザー管理者のみがユーザー パスワードをリセットできます。 グローバル管理者は、他の特権を持つ管理者のパスワードをリセットすることもできます。

**[パスワードのリセット] にオンプレミス統合ブレードが表示されていません**

- オンプレミス統合ブレードは、ハイブリッド環境だけで表示されます。つまり、パスワードの書き戻しを使用してオンプレミス ユーザーのパスワードを操作します。
- 次の場合、このブレードは表示されません。
    - パスワードの書き戻しを使用していない
    - パスワードの書き戻しのインストール/接続に問題がある
    - Azure AD Connect のインストール/接続に問題がある
    - パスワードの書き戻しに関する問題のトラブルシューティングの手順については、「[パスワードの書き戻しに関するトラブルシューティング](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)」セクションを参照してください。

**ユーザーのパスワードをリセットする方法がわかりません**

1. パスワードをリセットできる適切な管理者として Azure portal にサインインします。
1. [ユーザーおよびグループ] ブレードに移動し、**[すべてのユーザー]** を選択します。
1. 一覧からユーザーを選択します。
1. 選択したユーザーに対して、[**概要**] を選択し、コマンド バーで [**パスワードのリセット**] をクリックします。
1. 画面の指示に従います。
    - Azure portal で実行されるリセットのみ、パスワードの書き戻しをサポートします。

**Office 365 管理ポータルまたは Office 365 モバイル アプリケーションからオンプレミス ユーザーのパスワードをリセットしましたが、ユーザーがまだサインインできません**

このポータルでは、パスワードの書き戻しはサポートされていません。 Azure portal - portal.azure.com でユーザーのパスワードをリセットします。


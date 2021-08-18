---
title: Azure AD Connect でパスワードの書き戻しを有効にする
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 63304667cce67c48fd8bbeee52ff6d61d033ea38fd8d4c4d96c240847dab2cab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118209"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Azure AD Connect でパスワードの書き戻しを有効にする

セルフサービスのパスワード リセットの書き戻しを有効にするには、まず Azure AD Connect で書き戻しを有効にします。 Azure AD Connect サーバーから、次の手順を実行します。

1. Azure AD Connect サーバーにサインインし、**Azure AD Connect** 構成ウィザードを開始します。
2. [**ようこそ**] ページで、[**構成**] をクリックします。
3. **[追加のタスク]** ページで、**[同期オプションのカスタマイズ]** を選択し、**[次へ]** をクリックします。
4. **[Azure AD に接続]** ページで、Azure テナントのグローバル管理者の資格情報を入力して、**[次へ]** をクリックします。
5. [**ディレクトリの接続**] ページと[**ドメインと OU のフィルタ リング**] ページで、[**次へ**] をクリックします。
6. **[オプション機能]** ページで、**[パスワードの書き戻し]** の横のボックスを選択し、**[次へ]** をクリックします。
7. [**構成の準備完了**] ページで[**構成**] をクリックし、処理が完了するのを待ちます。
8. 構成の完了が表示されたら、[**終了**] をクリックします。

Azure AD Connect でパスワードの書き戻しが有効にして、書き戻し用に Azure AD SSPR を構成します。  SSPR でパスワードの書き戻しを有効にするには、次の手順を実行します。

1. グローバル管理者アカウントを使用して Azure ポータルにサインインします。
2. [**Azure Active Directory**] を検索して選択し、[**パスワードのリセット**] をクリックして、[**オンプレミスの統合**] をクリックします。
3. [**オンプレミスのディレクトリにパスワードをライトバックしますか?**] のオプションを [**はい**] に設定します。
4. [**パスワードをリセットせずにアカウントのロックを解除することをユーザーに許可しますか?**] オプションを [**はい**] に設定します。
5. 準備ができたら、[**保存**] をクリックします。

詳細については、「[オンプレミス環境への Azure Active Directory セルフサービスのパスワード リセットの書き戻しを有効にする](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)」をご覧ください。

> [!NOTE]
>  管理者が Azure ポータルでユーザーのパスワードをリセットしたとき、そのユーザーがフェデレーションされているかパスワードのハッシュが同期されている場合、パスワードがオンプレミスに書き戻されます。 この機能には Azure プレミアム ライセンス (P1 または P2) が必要であり、現在 Office 管理ポータルではサポートされていません。

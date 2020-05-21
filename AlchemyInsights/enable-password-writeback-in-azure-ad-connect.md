---
title: Azure AD Connect でパスワードの書き戻しを有効にする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: ab4b8692799d08363e1d726f72a3b80dcb598797
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2020
ms.locfileid: "44282050"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Azure AD Connect でパスワードの書き戻しを有効にする

セルフサービスのパスワード リセットの書き戻しを有効にするには、まず Azure AD Connect で書き戻しを有効にします。 Azure AD Connect サーバーから、次の手順を実行します。

1. Azure AD Connect サーバーにサインインし、**Azure AD Connect** 構成ウィザードを開始します。
2. [**ようこそ**] ページで、[**構成**] をクリックします。
3. **[追加のタスク]** ページで、**[同期オプションのカスタマイズ]** を選択し、**[次へ]** をクリックします。
4. **[Azure AD に接続]** ページで、Azure テナントのグローバル管理者の資格情報を入力して、[次へ] をクリックします。
5. [**ディレクトリの接続**] ページと[**ドメインと OU のフィルタ リング**] ページで、[**次へ**] をクリックします。
6. **[オプション機能]** ページで、**[パスワードの書き戻し]** の横のボックスを選択し、**[次へ]** をクリックします。
7. [**構成の準備完了**] ページで[**構成**] をクリックし、処理が完了するのを待ちます。
8. 構成の完了が表示されたら、[**終了**] をクリックします。

Azure AD Connect でパスワードの書き戻しが有効になったら、書き戻し用に Azure AD SSPR を構成します。  SSPR でパスワードの書き戻しを有効にするには、次の手順を実行します。

1. グローバル管理者アカウントを使用して Azure ポータルにサインインします。
2. [**Azure Active Directory **] を検索して選択し、[**パスワードのリセット**] をクリックして、[**オンプレミスの統合**] を選択します。
3. [**オンプレミスのディレクトリにパスワードをライトバックしますか?**] のオプションを [**はい**] に設定します。
4. [**パスワードをリセットせずにアカウントのロックを解除することをユーザーに許可しますか?**] オプションを [**はい**] に設定します。
5. 準備ができたら、[**保存**] をクリックします。

詳細については、「[オンプレミス環境への Azure Active Directory セルフサービスのパスワード リセットの書き戻しを有効にする](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)」をご覧ください。

---
title: Azure AD Connect でパスワードの書き戻しを有効にする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560445"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Azure AD Connect でパスワードの書き戻しを有効にする

セルフサービスのパスワード リセットの書き戻しを有効にするには、まず Azure AD Connect で書き戻しを有効にします。 Azure AD Connect サーバーから、次の手順を実行します。

1. Azure AD Connect サーバーにサインインし、**Azure AD Connect** 構成ウィザードを開始します。
2. [**ようこそ**] ページで、[**構成**] をクリックします。
3. **[追加のタスク]** ページで、**[同期オプションのカスタマイズ]** を選択し、**[次へ]** をクリックします。
4. **[Azure AD に接続]** ページで、Azure テナントのグローバル管理者の資格情報を入力して、**[次へ]** をクリックします。
5. [**ディレクトリの接続**] ページと[**ドメインと OU** のフィルタ リング] ページで、[**次へ**] をクリックします。
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
>  管理者が Azure ポータルでユーザーのパスワードをリセットした場合、そのユーザーがフェデレーションされているかパスワードのハッシュが同期されている場合、パスワードがオンプレミスに書き戻されます。 この機能は、現在Office 管理ポータルでサポートされていません。
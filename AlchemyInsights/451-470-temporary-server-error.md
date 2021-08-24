---
title: 451 4.7.0 一時的なサーバー エラー。 後でもう一度お試しください。 PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "57288373"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 一時的なサーバー エラー。 後でもう一度お試しください。 PRX4

Smarthost の「smtp.office365.com」で SMTP クライアント送信メソッドを使用してメールを送信する場合に、エラーが発生する場合があります:「451 4.7.0 一時的なサーバー エラー。 後でもう一度お試しください。 PRX4 はほとんどが一時的なものです。」 

SMTP クライアント送信方式では、メールを送信するためにライセンス済みのメールボックスが必要となるため、SMTP クライアント送信に共有メールボックスを使用していないことを確認してください。 ただし、共有メールボックスを使用しておらず、問題が解決しない場合は、以下を確認してください。

1. この PowerShell コマンドを実行して、使用するライセンス済みメールボックスでクライアント SMTP 送信を有効にします。

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    または

    1. [Microsoft 365 管理センター]、**[アクティブなユーザー]** の順に移動し、ユーザーを選択します。
    1. [メール] タブ、**[メール アプリ]** の順に移動し、**[メールアプリの管理]** を選択します。 
    1. **[認証済み SMTP]** 設定がオン (有効) になっていることを確認してください。
    1. [**変更の保存**] を選択します。
    
    組織全体で SMTP 認証を有効にするには、次のコマンドを実行します。

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **注意**: セキュリティ上の理由から、使用するメールボックスに対してのみ SMTP 認証を有効にすることをお勧めします。 ユーザー レベルの設定は、組織レベルの設定に上書きされます。

2. 「**セキュリティの既定値を有効にする**」を「**いいえ**」に切り替えて、「Azure セキュリティの既定値」を無効にします。

    1. Azure ポータルにセキュリティ管理者、条件付きアクセス管理者、またはグローバル管理者としてサインインします。
    1. [Azure Active Directory]**、 [プロパティ]** の順に移動し、**[セキュリティの既定の管理]** を選択します。
    1. **[セキュリティの既定値を有効にする]** の切り替えを **[いいえ]** に設定します。
    1. **[保存]** を選択します。

3. ライセンス付与されたメールボックスで使用する多要素認証 (MFA) を無効にします。

    1. Microsoft 365 管理センターに移動し、左側のナビゲーション メニューで、**[ユーザー]**、 > **[アクティブユーザー]** の順に選択します。
    1. **[アクティブ ユーザー]** ページで、**[多要素認証]** を選択します。
    1. ユーザーを選択し、**[多要素認証]** を無効にします。


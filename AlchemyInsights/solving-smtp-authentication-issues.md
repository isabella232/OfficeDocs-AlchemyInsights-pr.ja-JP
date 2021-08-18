---
title: SMTP 認証の有効化とトラブルシューティング
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
- "3000003"
- "5652"
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321758"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>SMTP 認証の有効化とトラブルシューティング

メールボックスの SMTP 認証を有効にしたい場合や、Microsoft 365 でデバイスやアプリケーションを認証してメールを中継しようとすると、5.7.57 または 5.7.3、5.7.139 のコードを含む「未認証のクライアント」、「認証は失敗しました」、「SmtpClientAuthentication」エラーが発生する場合は、以下の 3 つのアクションを実行して問題を解決してください。

1. 「**セキュリティの既定値を有効にする**」を「**いいえ**」に切り替えて、「[Azure セキュリティの既定値](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)」を無効にします。

    a. Azure ポータルにセキュリティ管理者、条件付きアクセス管理者、またはグローバル管理者としてサインインします。<BR/>
    b. [Azure Active Directory] >  **[プロパティ]** の順に移動します。<BR/>
    c. **[セキュリティの既定値を管理]** を選択します。<BR/>
    d. **[セキュリティの既定値を有効にする]** を **[いいえ]** に設定します。<BR/>
    e. **[保存]** を選択します。

2. ライセンス付与済みのメールボックスで、[[クライアント SMTP 送信]](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) を有効にします。

    a. Microsoft 365 管理センターから **[アクティブなユーザー]** に移動し、ユーザーを選択します。<BR/>
    b. [メール] タブを開き、**メール アプリ** の下にある **[メールアプリの管理]** を選択します。<BR/>
    d. **[認証済み SMTP]** チェックボックスがオン (有効) になっていることを確認してください。<BR/>
    e. **[変更の保存]** を選択します。<BR/>

3. ライセンス付与されたメールボックスで[多要素認証 (MFA) を無効にします](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa)。

    a. Microsoft 365 管理センターに移動し、左側のナビゲーション メニューで、**[ユーザー]** > **[アクティブ ユーザー]** を選択します。<BR/>
    b. **[多要素認証]** を選択します。<BR/>
    c. ユーザーを選択し、**[多要素認証]** を無効にします。<BR/>

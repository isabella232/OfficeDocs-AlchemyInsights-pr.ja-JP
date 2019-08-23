---
title: 監査ログのメールボックスでの外部メール転送を識別する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539106"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>メールボックスで外部電子メール転送がいつ構成されたかを特定する

Office 365 ユーザーがメールボックスで外部の電子メール転送を構成する場合、アクティビティは**メールボックスの設定**コマンドレットの一部として監査されます。 セキュリティ & コンプライアンスセンターで監査ログの検索を使用してアクティビティを確認できます。

1. [Office 365 セキュリティ & コンプライアンスセンター](https://protection.office.com/)にログインします。

2. [ **** > **監査ログ**の検索] ページに移動します。

3. [**開始日**] フィールドと [**終了日**] フィールドで日付範囲を選択します。 ユーザー名を指定する必要はありません。 [**アクティビティ**] フィールドが、**すべてのアクティビティの結果を表示**するように設定されていることを確認します。

4. **[検索]** をクリックします。

結果で、[**結果のフィルター処理**] をクリックし、[アクティビティフィルター] ボックスに「 **Set-Mailbox** 」と入力します。 結果で監査レコードを選択します。 **詳細**ポップアップで、[**詳細情報**] をクリックします。 アクティビティが電子メール転送に関連しているかどうかを判断するには、各監査レコードの詳細を参照する必要があります。

- **ObjectId**: 変更されたメールボックスのエイリアス値。

- **パラメーター**: _ForwardingSmtpAddress_は、ターゲットの電子メールアドレスを示します。

- **UserId**: **ObjectId**フィールドのメールボックスで電子メール転送を構成したユーザー。

詳細については、「[メールボックスのメール転送をセットアップするユーザーの特定](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)」を参照してください。

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
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383102"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>メールボックスで外部電子メール転送がいつ構成されたかを特定する

ユーザーがメールボックスで外部の電子メール転送を構成すると、アクティビティは**メールボックスの設定**コマンドレットの一部として監査されます。 セキュリティ & コンプライアンスセンターで監査ログの検索を使用してアクティビティを確認できます。

1. [Office 365 セキュリティ & コンプライアンスセンター](https://protection.office.com/)にログインする

2. [**検索と調査**] をクリックして、[**監査ログの検索**] を選択します。

3. [**開始日**] フィールドと [**終了日**] フィールドで日付範囲を選択します。 ユーザー名を指定する必要はありません。 [**アクティビティ**] フィールドが、**すべてのアクティビティの結果を表示**するように設定されていることを確認します。

4. **[検索]** をクリックします。

結果で、[**結果のフィルター処理**] をクリックし、[アクティビティフィルター] ボックスに「 **Set-Mailbox** 」と入力します。 結果で監査レコードを選択します。 **詳細**ポップアップで、[**詳細情報**] をクリックします。 アクティビティが電子メール転送に関連しているかどうかを判断するには、各監査レコードの詳細を参照する必要があります。

- **ObjectId**: 変更されたメールボックスのエイリアス値。

- **パラメーター**: _ForwardingSmtpAddress_は、ターゲットの電子メールアドレスを示します。

- **UserId**: **ObjectId**フィールドのメールボックスで電子メール転送を構成したユーザー。

詳細については、「[メールボックスのメール転送をセットアップするユーザーの特定](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)」を参照してください。

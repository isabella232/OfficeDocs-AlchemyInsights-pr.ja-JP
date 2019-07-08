---
title: 監査ログ内のメールボックスで外部のメール転送を特定する
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383102"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>外部のメール転送がメールボックスで構成された際に、それを特定する

ユーザーが外部のメール転送をメールボックスで構成すると、このアクティビティは **Set-Mailbox** コマンドレットの一部として監査されます。 セキュリティ/コンプライアンス センターで監査ログ検索を使用すると、アクティビティを表示できます。

1. [Office 365 セキュリティ/コンプライアンス センター](https://protection.office.com/)にログインします

2. [**検索と調査**] と [**監査ログ検索**]をクリックする。

3. [**開始日付**] と [**終了日付**] フィールドで日付範囲を選択します。 ユーザー名を指定する必要はありません。 [**アクティビティ**] フィールドが [**すべてのアクティビティの結果を表示**] と設定されていることを確認します。

4. [**検索**] をクリックします。

結果で、[**結果をフィルター**] をクリックし、[アクティビティ] フィルター ボックスに「**Set-Mailbox**」と入力します。 結果で、監査レコードを選択します。 [**詳細**] ポップアップから、[**詳細情報**]をクリックします。 アクティビティがメールの転送に関連しているかどうかを判断するには、各監査レコードの詳細を確認する必要があります。

- **ObjectId**: 変更されたメールボックスのエイリアス値。

- **パラメーター**: _ForwardingSmtpAddress_は、送信先のメール アドレスを示します。

- **UserId**: [**ObjectId**] フィールドのメールボックスでメール転送を構成したユーザー。

詳細については、「[メールボックスの電子メール転送を誰が設定したかを判別する](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)」を参照してください。

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
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539106"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>外部のメール転送がメールボックスで構成された際に、それを特定する

Office 365 のユーザーが外部のメール転送をメールボックスで構成すると、このアクティビティは **Set-Mailbox** コマンドレットの一部として監査されます。 セキュリティ/コンプライアンス センターで監査ログ検索を使用すると、アクティビティを表示できます。

1. [Office 365 セキュリティ/コンプライアンス センター](https://protection.office.com/) にログインします。

2. **[検索]** > **[監査ログの検索]** ページに移動します。

3. [**開始日**] と [**終了日**] フィールドで日付範囲を選択します。 ユーザー名を指定する必要はありません。 [**アクティビティ**] フィールドが [**すべてのアクティビティの結果を表示**] と設定されていることを確認します。

4. [**検索**] をクリックします。

結果で、[**結果をフィルター**] をクリックし、[アクティビティ] フィルター ボックスに「**Set-Mailbox**」と入力します。 結果で、監査レコードを選択します。 [**詳細**] ポップアップから、[**詳細情報**]をクリックします。 アクティビティがメールの転送に関連しているかどうかを判断するには、各監査レコードの詳細を確認する必要があります。

- **ObjectId**: 変更されたメールボックスのエイリアス値。

- **パラメーター**: _ForwardingSmtpAddress_は、送信先のメール アドレスを示します。

- **UserId**: [**ObjectId**] フィールドのメールボックスでメール転送を構成したユーザー。

詳細については、「[メールボックスの電子メール転送を誰が設定したかを判別する](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)」を参照してください。

---
title: 監査ログ内のメールボックスで外部のメール転送を特定する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331164"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>外部のメール転送がメールボックスで構成された際に、それを特定する

Microsoft 365 ユーザーが外部のメール転送をメールボックスで構成すると、このアクティビティは **Set-Mailbox** コマンドレットの一部として監査されます。 監査ログ検索を使用してアクティビティを確認できます。 手順は次のとおりです。

1. 次のいずれかの手順を実行します。
   - <https://compliance.microsoft.com> の Microsoft 365 コンプライアンス センターで、[**ソリューション**] \> [**監査**] の順に移動します。 または、[**監査**] ページに直接移動するには、<https://compliance.microsoft.com/auditlogsearch> を使用します。
   - <https://security.microsoft.com> の Microsoft 365 Defender ポータルで、[**監査**] に移動します。 または、[**監査**] ページに直接移動するには、<https://sip.security.microsoft.com/auditlogsearch> を使用します。

2. [**監査**] ページで、[**検索**] タブが選択されていることを確認してから、次の設定を構成します。
   - [**開始**] ボックスと [**終了**] ボックスで日付と時刻の範囲を選択します。
   - **[アクティビティ]** ボックスに **[すべてのアクティビティの結果を表示する]** が含まれていることを確認します。

3. 完了したら、[**検索**] をクリックします。 アクティビティは、新しい [**監査検索**] ページに表示されます。

4. 結果で、[**結果をフィルター**] をクリックし、[アクティビティ] フィルター ボックスに「**Set-Mailbox**」と入力します。

5. 結果で、監査レコードを選択します。 [**詳細**] ポップアップから、[**詳細情報**]をクリックします。 アクティビティがメールの転送に関連しているかどうかを判断するには、各監査レコードの詳細を確認する必要があります。

   - **ObjectId**: 変更されたメールボックスのエイリアス値。
   - **パラメーター**: _ForwardingSmtpAddress_ は、送信先のメール アドレスを示します。
   - **UserId**: [**ObjectId**] フィールドのメールボックスでメール転送を構成したユーザー。

詳細については、「[メールボックスの電子メール転送を誰が設定したかを判別する](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)」を参照してください。

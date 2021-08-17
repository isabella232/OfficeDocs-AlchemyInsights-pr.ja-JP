---
title: メールボックスに転送を設定したユーザーとその方法を確認する
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895184"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>メールボックスに転送を設定したユーザーとその方法を確認する

外部転送がメールボックスに設定されている場合、アクティビティは **Set-Mailbox** コマンドレットの一部として監査されます。 監査ログでアクティビティを見つける方法は次のとおりです。

1. 次のいずれかの操作を実行します。
   - [ソリューションの <https://compliance.microsoft.com> Microsoft 365 コンプライアンス センター] の [ソリューション監査]**に** \> **移動します**。 または、[監査] ページに直接 **移動するには** 、 を使用します <https://compliance.microsoft.com/auditlogsearch> 。
   - [監査] Microsoft 365 Defenderポータル <https://security.microsoft.com> で、[監査] に **移動します**。 または、[監査] ページに直接 **移動するには** 、 を使用します <https://security.microsoft.com/auditlogsearch> 。

   > [!NOTE]
   > 監査を有効にする必要があるという通知が表示された場合は、先に進んで今すぐ有効にしてください。 この機能が有効になっていない場合、検索結果は前の日付からデータを取得できません。

2. [監査 **] ページで** 、[検索] タブ **が** 選択されているのを確認し、次の設定を構成します。
   - [開始] ボックスと [終了] ボックスで日付と時刻 **の範囲を** 選択します。
   - [アクティビティ] **ボックスに** [すべてのアクティビティ **の結果を表示する] が含まれているか確認します**。

3. 完了したら、[検索] を **クリックします**。 新しい [監査] 検索ページ **にアクティビティが表示** されます。

4. 結果で、[アクティビティ] 列 **をクリック** して結果を並べ替え **、Set-Mailbox** エントリを探します。

5. 結果でアクティビティを選択して詳細フライアウトを開きます。 各監査レコードの詳細を確認して、アクティビティがメール転送に関連しているかどうかを判断する必要があります。
   - **ObjectId**: 変更されたメールボックスのエイリアス値。
   - **パラメーター**: _ForwardingSmtpAddress_ は、送信先のメール アドレスを示します。
   - **UserId**: [**ObjectId**] フィールドのメールボックスでメール転送を構成したユーザー。

詳細については、「[メールボックスの電子メール転送を誰が設定したかを判別する](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)」を参照してください。

---
title: 削除されたイベントの監査ログを読み取る
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324738"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>削除されたイベントの監査ログを読み取る

手順は次のとおりです。

1. 次のいずれかの操作を実行します。
   - [ソリューションの <https://compliance.microsoft.com> Microsoft 365 コンプライアンス センター] の [ソリューション監査]**に** \> **移動します**。 または、[監査] ページに直接 **移動するには** 、 を使用します <https://compliance.microsoft.com/auditlogsearch> 。
   - [監査] Microsoft 365 Defenderポータル <https://security.microsoft.com> で、[監査] に **移動します**。 または、[監査] ページに直接 **移動するには** 、 を使用します <https://security.microsoft.com/auditlogsearch> 。

    **注**: 機能を有効にする必要があるという通知が表示された場合は、次に進んでオンにします。 この機能が有効になっていない場合、検索結果は前の日付からデータを取得できません。

2. [監査 **] ページの** [検索] **タブで** 、次の設定を構成します。
   - **日付と時刻の範囲**: [開始] ボックスと [終了] ボックスで日付/時刻 **の範囲****を** 選択します。
   - **アクティビティ**: メールボックス アクティビティ **Exchange入力し、** 次の値を選択します。
     - **削除済みアイテム フォルダーからのメッセージの削除**
     - **削除済みアイテム フォルダーへのメッセージの移動**

       完了したら、ウィンドウの外側をクリックして、**[アクティビティ]** ウィンドウを最小化します。

   - **ユーザー**: 空白の既定値を受け入れて、すべてのユーザーの結果を返すか、1 つ以上のユーザーを入力します。

3. 完了したら、[検索] を **クリックします**。 新しい [監査] 検索ページ **にアクティビティが表示** されます。

4. 結果でアクティビティを選択して詳細フライアウトを開きます。 削除された項目に関する追加情報(件名、項目が削除されたときの場所など) は、 [**対象アイテム**] フィールドに表示されます。

   **注**: 監査ログ機能を使用して削除済みアイテムを復元できない。 削除済みアイテムを復元するには、「削除された電子メール メッセージを復元する」を参照[Outlook on the web。](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)

詳細については、「監査ログを [検索して一般的なサポートの問題を調査する」を参照してください](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。

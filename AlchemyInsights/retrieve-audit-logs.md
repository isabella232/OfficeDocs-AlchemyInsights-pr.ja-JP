---
title: 監査ログを取得する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/16/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10964"
- "3100005"
ms.openlocfilehash: 6ca61775d18fb5501911fb3334ef499ff1f06a6b42634367eaf546fc322f822c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889651"
---
# <a name="retrieve-the-audit-logs"></a>監査ログを取得する

最初に監査ログを開いたときは、空になっています。 そこに何があるかを確認するには、検索を行う必要があります。 すべてのアクティビティを検索する一般的な方法は、次のとおりです。

1. 次のいずれかの手順を実行します。
   - <https://compliance.microsoft.com> の Microsoft 365 コンプライアンス センターで、[**ソリューション**] \> [**監査**] の順に移動します。 または、[**監査**] ページに直接移動するには、<https://compliance.microsoft.com/auditlogsearch> を使用します。
   - <https://security.microsoft.com> の Microsoft 365 Defender ポータルで、[**監査**] に移動します。 または、[**監査**] ページに直接移動するには、<https://sip.security.microsoft.com/auditlogsearch> を使用します。

2. [**監査**] ページで、[**検索**] タブが選択されていることを確認してから、次の設定を構成します。
   - **日付と時刻の範囲**: [**開始**] ボックスと [**終了**] ボックスで日付と時刻の範囲を選択します。
   - **アクティビティ**: [**すべてのアクティビティの結果を表示する**] が選択されていることを確認します。
   - **ユーザー**: 空白の既定値を受け入れてすべてのユーザーの結果を返すか、1 人以上のユーザーを入力します。

3. 完了したら、[**検索**] をクリックします。 アクティビティは、新しい [**監査検索**] ページに表示されます。

4. 結果で、[**結果をフィルター**] をクリックし、[アクティビティ] フィルター ボックスに「**Set-Mailbox**」と入力します。

5. 結果で、監査レコードを選択します。 [**詳細**] ポップアップで、[**詳細情報**] をクリックし、クライアントやアクションを実行したユーザーなどの詳細情報を表示します。

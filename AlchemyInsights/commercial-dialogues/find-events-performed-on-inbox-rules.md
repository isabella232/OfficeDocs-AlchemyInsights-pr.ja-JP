---
title: 受信トレイのルールで実行されたイベントを検索する
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
ms.openlocfilehash: 14a5a18bc1422572db567c9533fefe5a7e0120afd64df4a64623038cc063ce93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058655"
---
# <a name="find-events-performed-on-inbox-rules"></a>受信トレイのルールで実行されたイベントを検索する

受信トレイのルールが作成、変更、または削除されると、イベントは監査ログに記録されます。 レビューする方法は、次のとおりです。

1. [Office 365 セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/p/?linkid=2077143)に移動します。
1. [検索] > [ログ検索の監査] を選択します。

    > [!NOTE]
    > 監査を有効にする必要があるという通知が表示された場合は、先に進んで今すぐ有効にしてください。 この機能が有効になっていない場合、検索結果は前の日付からデータを取得できません。
1. [アクティビティ] フィールドを選択してExchange メールボックス アクティビティを見つけ、[新規] - [受信トレイのルール] [Outlook Web App から受信トレイの作成]ルールを選択します。  完了したら、ウィンドウの外側をクリックして、[アクティビティ] ウィンドウを最小化します。
1. 日付範囲を指定し、[ユーザー] フィールドで、調査するユーザーのユーザー名を選択します。 一度に複数のエントリを選択できます。
1. [検索] を選択します。 アクティビティは [結果] の下に表示されます。
1. 詳細を表示するには、アクティビティを選択してから、[詳細情報] を選択します。 [パラメータ] セクションで、ルールの名前、設定された条件、およびルールが実行するアクションを確認できます。

詳細については、「Office 365 監査ログを検索して一般的なシナリオのトラブルシューティングを行う」をご覧ください。
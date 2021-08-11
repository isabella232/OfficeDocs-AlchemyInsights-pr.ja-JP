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
ms.openlocfilehash: 8d656d5660b7c6e6d32d32a06c3dbf49c45e4ca04c4422128f1c4ea62413afa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967338"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>削除されたイベントの監査ログを読み取る

手順は次のとおりです。

1. [Office 365 セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/p/?linkid=2077143)に移動します。
1. **[検索]** > [**[監査ログ検索]**](https://go.microsoft.com/fwlink/?linkid=2103759) を選択します。
    > [!NOTE]
    > この機能を有効にする必要があるという通知が表示された場合は、先に進んで今すぐ有効にしてください。 この機能が有効になっていない場合、検索結果は前の日付からデータを取得できません。
1. **[アクティビティ]** を選択し、**[Exchange メール ボックス アクティビティ]** を検索します。 **[削除済みアイテムフォルダからの削除済みメッセージ]** および **[削除済みアイテム フォルダに移動済みのメッセージ]** オプションを選択します。 完了したら、ウィンドウの外側をクリックして、**[アクティビティ]** ウィンドウを最小化します。
1. 日付範囲を指定し、**[ユーザー]** ボックス、調査するユーザーのユーザー名を選択します。 一度に複数のエントリを選択できます。
1. **[検索]** を選択します。 アクティビティは **[結果]** の下に表示されます。
1. 詳細を表示するには、アクティビティを選択してから、**[詳細情報]** を選択します。 削除された項目に関する追加情報(件名、項目が削除されたときの場所など) は、 [**対象アイテム**] フィールドに表示されます。
    > [!NOTE]
    > 監査ログ機能を使用して、削除したアイテムを復元することはできません。 削除済みアイテムを復元する方法については、「[Outlook Web App で削除済みのアイテムやメールを復元する](https://go.microsoft.com/fwlink/?linkid=2103759)」をご覧ください。

詳細については、「[Office 365 監査ログを検索して一般的なシナリオのトラブルシューティングを行う](https://go.microsoft.com/fwlink/?linkid=2103944)」をご覧ください。

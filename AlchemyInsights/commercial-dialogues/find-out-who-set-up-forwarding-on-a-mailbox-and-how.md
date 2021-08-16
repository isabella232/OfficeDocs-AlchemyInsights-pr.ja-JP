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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988209"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>メールボックスに転送を設定したユーザーとその方法を確認する

メールボックスに外部転送が設定されている場合、アクティビティは Set-Mailbox コマンドレットの一部として監査されます。 監査ログでアクティビティを見つける方法は次のとおりです。

1. [Office 365 セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/p/?linkid=2077143)に移動します。
1. **[検索]**> **[監査ログ検索]** を選択します。
    > [!NOTE]
    > 監査を有効にする必要があるという通知が表示された場合は、先に進んで今すぐ有効にしてください。 この機能が有効になっていない場合、検索結果は前の日付からデータを取得できません。
1. [**アクティビティ**] フィールドが [**すべてのアクティビティの結果を表示**] (既定) と設定されていることを確認してください。 日付範囲を指定します。 ユーザー名を指定する必要はありません。
1. **[検索]** を選択します。 アクティビティは **[結果]** の下に表示されます。
1. **[結果をフィルター]** を選択し、[**アクティビティ** フィルター] フィールドに **Set-mailbox** と入力します。 これにより、すべての **Set-Mailbox** アクティビティが返されます。
1. 詳細を表示するには、アクティビティを選択してから、**[詳細情報]** を選択します。 **[パラメータ]** の下に、メール ボックスに設定された転送メール アドレスが表示されます。 **[UserID]** は、メール ボックスに外部転送を設定したユーザーを表します。
詳細については、「[Office 365 監査ログを検索して一般的なシナリオのトラブルシューティングを行う](https://go.microsoft.com/fwlink/?linkid=2103944)」をご覧ください。
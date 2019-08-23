---
title: 監査ログで受信トレイルールのアクティビティを識別する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539177"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>監査ログで受信トレイルールのアクティビティを識別する

Office 365 セキュリティ & コンプライアンスセンターで監査ログの検索を使用して、受信トレイルールのイベント (受信トレイルールの作成、変更、および削除) を表示できます。

1. [Office 365 セキュリティ & コンプライアンスセンター](https://protection.office.com/)にログインします。

2. [ **** > **監査ログ**の検索] ページに移動します。

3. [**開始日**] フィールドと [**終了日**] フィールドで日付範囲を選択します。

4. [ **Exchange メールボックスアクティビティ**] で、[**アクティビティ**] フィールドが [**新規-受信トレイルールの作成/変更/有効化/有効化/無効化**] に設定されていることを確認します。

5. **[検索]** をクリックします。

結果から、監査レコードを選択します。 詳細ポップアップで、[**詳細情報**] をクリックします。 受信トレイルールの設定に関する情報は、[**パラメーター** ] フィールドに表示されます。

詳細については、「[ユーザーが受信トレイルールを作成したか](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)どうかの判断」を参照してください。

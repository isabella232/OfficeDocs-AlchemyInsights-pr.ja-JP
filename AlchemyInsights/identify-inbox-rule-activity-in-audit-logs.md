---
title: 監査ログで受信トレイのルール アクティビティを特定する
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
ms.openlocfilehash: 51c25897223371a6dcc94c948955107ce74b0e8e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383030"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>監査ログで受信トレイのルール アクティビティを特定する

セキュリティ/コンプライアンス センターで監査ログの検索を使用して、受信トレイのルールのイベント (受信トレイのルールの作成、変更、および削除) を表示することができます。

1. [Office 365 セキュリティ/コンプライアンス センター](https://protection.office.com/)にログインする

2. [**検索と調査**] と [**監査ログ検索**]をクリックする。

3. [**開始日**] と [**終了日**] フィールドで日付範囲を選択します。

4. [**Exchange メールボックスのアクティビティ**] の下で、[**アクティビティ**] フィールドが [**New-InboxRule 受信トレイのルールの作成/変更/有効化/無効化**] に設定されていることを確認します。

5. [**検索**] をクリックします。

結果から、[監査レコード] を選択します。 詳細ポップアップから、 [**詳細情報**] をクリックします。 受信トレイのルール設定に関する情報は、[**パラメーター**] フィールドに表示されます。

詳細については、「[ユーザーが受信トレイ ルールを作成したかどうかを判別する](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)」を参照してください。

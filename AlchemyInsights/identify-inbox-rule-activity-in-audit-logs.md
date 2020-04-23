---
title: 監査ログで受信トレイのルール アクティビティを特定する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716429"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>監査ログで受信トレイのルール アクティビティを特定する

Microsoft 365 セキュリティ & コンプライアンスセンターで監査ログの検索を使用して、受信トレイルールイベント (受信トレイルールの作成、変更、および削除) を表示することができます。

1. [Microsoft 365 セキュリティ & コンプライアンスセンター](https://protection.office.com/)にログインします。

2. **[検索]** > **[監査ログの検索]** ページに移動します。

3. [**開始日**] と [**終了日**] フィールドで日付範囲を選択します。

4. [**Exchange メールボックスのアクティビティ**] の下で、[**アクティビティ**] フィールドが [**New-InboxRule 受信トレイのルールの作成/変更/有効化/無効化**] に設定されていることを確認します。

5. [**検索**] をクリックします。

結果から、[監査レコード] を選択します。 詳細ポップアップから、 [**詳細情報**] をクリックします。 受信トレイのルール設定に関する情報は、[**パラメーター**] フィールドに表示されます。

詳細については、「[ユーザーが受信トレイ ルールを作成したかどうかを判別する](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)」を参照してください。

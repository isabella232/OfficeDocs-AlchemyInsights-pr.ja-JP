---
title: 監査ログで受信トレイのルール アクティビティを特定する
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891300"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>監査ログで受信トレイのルール アクティビティを特定する

Microsoft 365 コンプライアンス センターで、監査ログの検索を使用して、受信トレイのルールのイベント (受信トレイのルールの作成、変更、および削除) を表示することができます。

1. 次のいずれかの手順を実行します。
   - <https://compliance.microsoft.com> の Microsoft 365 コンプライアンス センターで、**[ソリューション]** \> **[監査]** の順に移動します。 または、**[監査]** ページに直接移動するには、<https://compliance.microsoft.com/auditlogsearch> を使用します。
   - <https://security.microsoft.com> の Microsoft 365 Defender ポータルで、**[監査]** に移動します。 または、**[監査]** ページに直接移動するには、<https://security.microsoft.com/auditlogsearch> を使用します。

2. **[監査]** ページの **[検索]** タブで、次の設定を構成します。
   - **日付と時刻の範囲**: **[開始]** ボックスと **[終了]** ボックスで日付と時刻の範囲を選択します。
   - **アクティビティ**: 次の値の 1 つ以上を選択します。
     - **Outlook Web App の New-InboxRule 作成受信トレイ ルール**
     - **Outlook Web App の Set-InboxRule 変更ルール**。
     - **Outlook クライアントからの受信トレイ ルールの更新**

3. 完了したら、**[検索]** をクリックします。 アクティビティは、新しい **[監査検索]** ページに表示されます。

4. 結果でアクティビティを選択して、詳細ポップアップを開きます。 受信トレイのルール設定に関する情報は、**[パラメーター]** フィールドに表示されます。

詳細については、「[ユーザーが受信トレイ ルールを作成したかどうかを判別する](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)」を参照してください。

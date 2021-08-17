---
title: すべてのユーザーのアクティビティを調査する
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: d05c8f02efc3bb92865880ea4a2338abaf7d70254f0b4bbfb566423e62b391dd
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898801"
---
# <a name="investigate-all-the-users-activities"></a>すべてのユーザーのアクティビティを調査する

その手順は次のとおりです。

1. 次のいずれかの操作を実行します。
   - [ソリューションの <https://compliance.microsoft.com> Microsoft 365 コンプライアンス センター] の [ソリューション監査]**に** \> **移動します**。 または、[監査] ページに直接 **移動するには** 、 を使用します <https://compliance.microsoft.com/auditlogsearch> 。
   - [監査] Microsoft 365 Defenderポータル <https://security.microsoft.com> で、[監査] に **移動します**。 または、[監査] ページに直接 **移動するには** 、 を使用します <https://security.microsoft.com/auditlogsearch> 。

    > [!NOTE]
    > この機能を有効にする必要があるという通知が表示された場合は、先に進んで今すぐ有効にしてください。 この機能が有効になっていない場合、検索結果は前の日付からデータを取得できません。

2. [監査 **] ページの** [検索] **タブで** 、次の設定を構成します。
   - **日付と時刻の範囲**: [開始] ボックスと [終了] ボックスで日付/時刻 **の範囲****を** 選択します。
   - **アクティビティ**: 特定のアクティビティに興味がある場合は、一覧からアクティビティを選択します。それ以外の場合、既定値 [すべてのアクティビティの結果を表示 **する] は、すべてのアクティビティ** を返します。
   - **ユーザー**: 空白の既定値を受け入れて、すべてのユーザーの結果を返すか、1 つ以上のユーザーを入力します。

3. 完了したら、[検索] を **クリックします**。 新しい [監査] 検索ページ **にアクティビティが表示** されます。 IP アドレス、ユーザー、**および****アクティビティ** 名 **が表示** されます。

4. 結果をダウンロードするには、[すべての結果をダウンロード **する]** \> **を選択します**。

5. 結果でアクティビティを選択して詳細フライアウトを開きます。

詳細については、「監査ログを [検索して一般的なサポートの問題を調査する」を参照してください](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。

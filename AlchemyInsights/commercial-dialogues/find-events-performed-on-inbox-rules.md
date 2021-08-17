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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313504"
---
# <a name="find-events-performed-on-inbox-rules"></a>受信トレイのルールで実行されたイベントを検索する

受信トレイのルールが作成、変更、または削除されると、イベントは監査ログに記録されます。 レビューする方法は、次のとおりです。

1. 次のいずれかの操作を実行します。
   - [ソリューションの <https://compliance.microsoft.com> Microsoft 365 コンプライアンス センター] の [ソリューション監査]**に** \> **移動します**。 または、[監査] ページに直接 **移動するには** 、 を使用します <https://compliance.microsoft.com/auditlogsearch> 。
   - [監査] Microsoft 365 Defenderポータル <https://security.microsoft.com> で、[監査] に **移動します**。 または、[監査] ページに直接 **移動するには** 、 を使用します <https://security.microsoft.com/auditlogsearch> 。

    **注**: 監査を有効にする必要があるという通知が表示された場合は、次に進んでオンにしてください。 この機能が有効になっていない場合、検索結果は前の日付からデータを取得できません。
1. [アクティビティ] フィールドを選択してExchange メールボックス アクティビティを見つけ、[新規] - [受信トレイのルール] [Outlook Web App から受信トレイの作成]ルールを選択します。  完了したら、ウィンドウの外側をクリックして、[アクティビティ] ウィンドウを最小化します。
1. 日付範囲を指定し、[ユーザー] フィールドで、調査するユーザーのユーザー名を選択します。 一度に複数のエントリを選択できます。
1. [検索] を選択します。 アクティビティは [結果] の下に表示されます。
1. 詳細を表示するには、アクティビティを選択してから、[詳細情報] を選択します。 [パラメータ] セクションで、ルールの名前、設定された条件、およびルールが実行するアクションを確認できます。

2. [監査 **] ページの** [検索] **タブで** 、次の設定を構成します。
   - **日付と時刻の範囲**: [開始] ボックスと [終了] ボックスで日付/時刻 **の範囲****を** 選択します。
   - **アクティビティ**: **[New-InboxRule] [受信トレイ ルールを作成する] を選択Outlook Web App**

3. 完了したら、[検索] を **クリックします**。 新しい [監査] 検索ページ **にアクティビティが表示** されます。

4. 結果でアクティビティを選択して詳細フライアウトを開きます。 [パラメーター **] セクション** には、ルールの名前、条件セット、およびルールが実行するアクションが表示されます。

詳細については、「監査ログを [検索して一般的なサポートの問題を調査する」を参照してください](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。

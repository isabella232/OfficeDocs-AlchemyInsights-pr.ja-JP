---
title: 監査ログを取得する
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
ms.openlocfilehash: a653347e951109adaa873554d98c10b497c21caa68403a083543c806c310e079
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893596"
---
# <a name="retrieve-the-audit-logs"></a>監査ログを取得する

監査ログを最初に開くと、空になります。 そこに何があるかを確認するには、検索を行う必要があります。 すべてのアクティビティを検索する一般的な方法は、次のとおりです。

1. 次のいずれかの操作を実行します。
   - [ソリューションの <https://compliance.microsoft.com> Microsoft 365 コンプライアンス センター] の [ソリューション監査]**に** \> **移動します**。 または、[監査] ページに直接 **移動するには** 、 を使用します <https://compliance.microsoft.com/auditlogsearch> 。
   - [監査] Microsoft 365 Defenderポータル <https://security.microsoft.com> で、[監査] に **移動します**。 または、[監査] ページに直接 **移動するには** 、 を使用します <https://security.microsoft.com/auditlogsearch> 。

2. [監査 **] ページの** [検索] **タブで** 、次の設定を構成します。
   - **日付と時刻の範囲**: [開始] ボックスと [終了] ボックスで日付/時刻 **の範囲****を** 選択します。
   - **[アクティビティ**] : **[すべてのアクティビティの結果を表示する] が** 選択されているのを確認します。
   - **ユーザー**: 空白の既定値を受け入れて、すべてのユーザーの結果を返すか、1 つ以上のユーザーを入力します。

3. 完了したら、[検索] を **クリックします**。 新しい [監査] 検索ページ **にアクティビティが表示** されます。

4. 結果でアクティビティを選択して詳細フライアウトを開きます。 クライアント、アクションを実行したユーザーなどの詳細情報が表示されます。

詳細については、「監査ログを [検索して一般的なサポートの問題を調査する」を参照してください](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。

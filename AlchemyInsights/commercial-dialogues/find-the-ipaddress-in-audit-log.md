---
title: 監査ログで IP アドレスを見つける
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
ms.openlocfilehash: 258e92368b8a33e8ea807f0cb9af90132c86ed5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58303582"
---
# <a name="find-the-ip-address-in-audit-log"></a>監査ログで IP アドレスを見つける

ユーザーまたは管理者によって実行されたアクティビティに対応する IP アドレスが監査ログに表示されます。 クライアント情報も記録されます。 IP アドレスを特定する方法は次のとおりです。

1. 次のいずれかの操作を実行します。
   - [ソリューションの <https://compliance.microsoft.com> Microsoft 365 コンプライアンス センター] の [ソリューション監査]**に** \> **移動します**。 または、[監査] ページに直接 **移動するには** 、 を使用します <https://compliance.microsoft.com/auditlogsearch> 。
   - [監査] Microsoft 365 Defenderポータル <https://security.microsoft.com> で、[監査] に **移動します**。 または、[監査] ページに直接 **移動するには** 、 を使用します <https://security.microsoft.com/auditlogsearch> 。

    **注**: 監査を有効にする必要があるという通知が表示された場合は、次に進んでオンにしてください。 この機能が有効になっていない場合、検索結果は前の日付からデータを取得できません。

2. [監査 **] ページで** 、[検索] タブ **が** 選択されているのを確認し、次の設定を構成します。
   - **日付と時刻の範囲**: [開始] ボックスと [終了] ボックスで日付/時刻 **の範囲****を** 選択します。
   - **アクティビティ**: 特定のアクティビティに興味がある場合は、一覧からアクティビティを選択します。それ以外の場合、既定値 **[すべてのアクティビティの結果** を表示する] は、すべてのアクティビティが返されます。 特定のアクティビティを選択できない場合があります。ただし、[すべてのアクティビティの結果を表示する] が選択されている場合は、これらの **監査項目が** 返されます。
   - **ユーザー**: 空白の既定値を受け入れて、すべてのユーザーの結果を返すか、1 つ以上のユーザーを入力します。

3. 完了したら、[検索] を **クリックします**。 新しい [監査] 検索ページ **にアクティビティが表示** されます。

4. 結果で、[**結果をフィルター**] をクリックし、[アクティビティ] フィルター ボックスに「**Set-Mailbox**」と入力します。

5. 結果で監査レコードを選択して、[詳細] フライアウト **を** 開きます。

詳細については、「監査ログを [検索して一般的なサポートの問題を調査する」を参照してください](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。

---
title: 予定表イベントが表示されない、または更新されない
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837686"
---
# <a name="calendar-events-missing-or-not-updating"></a>予定表イベントが表示されない、または更新されない

予定表アイテムが表示されない、または更新されない場合は、Outlook の [予定表] フォルダーのプロパティにあるアイテム数の確認から始めます。 

1. 影響を受けたユーザーの **[予定表]** フォルダーを右クリックし、**[プロパティ]** を選択します。

1. **[同期]** タブを選択します。

[サーバー] フォルダーと [オフライン] フォルダーの間でアイテム数が同じではない場合は次のように操作します。

1.  **[予定表]** フォルダーを強調表示します。

1.  **[送信]**/**[受信]** タブに移動し、**[フォルダーを更新する]** を選択します。

予定表がまだ更新されないか、イベントが表示されない場合は、[Microsoft ダウンロード センター](https://www.microsoft.com/download/details.aspx?id=28786)から Outlook 用予定表チェック ツールをダウンロードします。 予定表フォルダーに 5000 個を超えるアイテムが含まれるかどうかを確認します。これが原因で、予定表会議が更新されない現象や会議のエラーなどが発生する可能性があります。 

詳細については、「[キャッシュ モードの .ost ファイルまたは .pst ファイル内のアイテムまたはフォルダーが多すぎる場合の Outlook のパフォーマンスの問題](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders)」を参照してください。
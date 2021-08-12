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
ms.openlocfilehash: af45345bc8779489f5e00dcaee136103e674068e29c77d8c536d012f475c33c5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968706"
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
---
title: 1332 OWA - 受信トレイのルールがメールボックスに対して実行されていません
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
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040907"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>受信トレイのルールが期待どおりに機能しません

Outlook on the web で次の設定を確認する:

- メッセージは、自動的に受信トレイのルールに 1 回だけ従うように、リダイレクト、転送、または返信できます。リダイレクト ルール (受信トレイのルールまたはメール フロー ルール。トランスポート ルールとも呼ばれる) では、メッセージに最大 10 個の転送受信者を追加できます。詳細については、[ジャーナル、トランスポート、および受信トレイのルールの制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)に関するページを参照してください。

- 受信トレイのルールは、代替ジャーナリング メールボックスでは機能しません。代替ジャーナリング メールボックスの詳細については、[代替ジャーナリング メールボックス](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)に関するページを参照してください。

これらの問題を修正するには、「[KB 2829319](https://support.microsoft.com/kb/2829319)」を参照してください。

以前の問題が該当しない場合は、Microsoft サポートに問題をエスカレーションする前に、受信トレイのルールの診断レポートを実行します。

1. Outlook on the web でメールボックスを開いて、 <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **[設定]** > **[Outlook のすべての設定を表示]** > **[メール]** > **[ルール]** の順にクリックします。

2. ページの下部にある **[ルールが正しく機能しない場合は、ここをクリックして診断レポートを生成してください]** をクリックします。

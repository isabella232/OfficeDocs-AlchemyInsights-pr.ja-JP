---
title: 1332 OWA - 受信トレイのルールがメールボックスに対して実行されていません
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858749"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>受信トレイのルールが期待どおりに機能しません

次の設定を確認してください。

- メッセージは、自動的に受信トレイのルールに 1 回だけ従うように、リダイレクト、転送、または返信できます。リダイレクト ルール (受信トレイのルールまたはメール フロー ルール。トランスポート ルールとも呼ばれる) では、メッセージに最大 10 個の転送受信者を追加できます。詳細については、[ジャーナル、トランスポート、および受信トレイのルールの制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)に関するページを参照してください。

- 受信トレイのルールは、代替ジャーナリング メールボックスでは機能しません。代替ジャーナリング メールボックスの詳細については、[代替ジャーナリング メールボックス](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)に関するページを参照してください。

これらの問題を修正するには、「[KB 2829319](https://support.microsoft.com/kb/2829319)」を参照してください。

以前の問題が該当しない場合は、Microsoft サポートに問題をエスカレーションする前に、受信トレイのルールの診断レポートを実行します。

1. Outlook on the web でメールボックスを開き、**[設定]**、**[オプション]**、**[メールの整理]**、**[受信トレイのルール]** の順にクリックします。

2. ページの下部にある **[ルールが正しく機能しない場合は、ここをクリックして診断レポートを生成してください]** をクリックします。

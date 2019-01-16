---
title: 1332 OWA の受信トレイ ルールが実行していないメールボックスの
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28298052"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>受信トレイ ルールが期待どおりに動作しません。

次の設定を確認します。
  
- 転送、または自動的に受信トレイ ルールに基づいて 1 回だけ返信、メッセージをリダイレクトできます。(受信トレイのルールまたはメール フロー ルール、トランスポート ルールとも呼ばれます) のリダイレクトのルールは、メッセージを 10 個の転送先の受信者の最大を追加できます。詳細については、[仕訳帳、トランスポート、および受信トレイ ルールの制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)を参照してください。
    
- 代替ジャーナリング メールボックスの受信トレイのルールが機能しません。代替ジャーナリング メールボックスの詳細については、[代替ジャーナリング メールボックス](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)を参照してください。
    
これらの問題を修正するのには、 [KB 2829319](https://support.microsoft.com/kb/2829319)を参照してください。
  
以前の問題が適用されない場合は、Microsoft サポートにこの問題をエスカレートする前に、受信トレイ ルールの診断レポートを実行します。
  
1. Web 上の Outlook でメールボックスを開くし、[**設定**] をクリックして\>**オプション** \> **整理電子メール** \> **受信トレイのルール**です。
    
2. ページの下部には、**ルールは、診断レポートを生成するのにはここをクリックして動作していないかどうか**] をクリックします。
    


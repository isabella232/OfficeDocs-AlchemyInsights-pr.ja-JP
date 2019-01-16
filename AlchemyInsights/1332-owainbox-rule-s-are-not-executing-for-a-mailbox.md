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
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="bb6c7-102">受信トレイ ルールが期待どおりに動作しません。</span><span class="sxs-lookup"><span data-stu-id="bb6c7-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="bb6c7-103">次の設定を確認します。</span><span class="sxs-lookup"><span data-stu-id="bb6c7-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="bb6c7-p101">転送、または自動的に受信トレイ ルールに基づいて 1 回だけ返信、メッセージをリダイレクトできます。(受信トレイのルールまたはメール フロー ルール、トランスポート ルールとも呼ばれます) のリダイレクトのルールは、メッセージを 10 個の転送先の受信者の最大を追加できます。詳細については、[仕訳帳、トランスポート、および受信トレイ ルールの制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb6c7-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="bb6c7-p102">代替ジャーナリング メールボックスの受信トレイのルールが機能しません。代替ジャーナリング メールボックスの詳細については、[代替ジャーナリング メールボックス](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb6c7-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="bb6c7-109">これらの問題を修正するのには、 [KB 2829319](https://support.microsoft.com/kb/2829319)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb6c7-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="bb6c7-110">以前の問題が適用されない場合は、Microsoft サポートにこの問題をエスカレートする前に、受信トレイ ルールの診断レポートを実行します。</span><span class="sxs-lookup"><span data-stu-id="bb6c7-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="bb6c7-111">Web 上の Outlook でメールボックスを開くし、[**設定**] をクリックして\>**オプション** \> **整理電子メール** \> **受信トレイのルール**です。</span><span class="sxs-lookup"><span data-stu-id="bb6c7-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="bb6c7-112">ページの下部には、**ルールは、診断レポートを生成するのにはここをクリックして動作していないかどうか**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="bb6c7-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    


---
title: 1332 OWA - 受信トレイのルールがメールボックスに対して実行されていません
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 7d1848830847fc6722da20e09a4875f49bf02bd3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35360922"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="123c4-102">受信トレイのルールが期待どおりに機能しません</span><span class="sxs-lookup"><span data-stu-id="123c4-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="123c4-103">次の設定を確認してください。</span><span class="sxs-lookup"><span data-stu-id="123c4-103">Verify the following settings:</span></span>

- <span data-ttu-id="123c4-p101">メッセージは、自動的に受信トレイのルールに 1 回だけ従うように、リダイレクト、転送、または返信できます。リダイレクト ルール (受信トレイのルールまたはメール フロー ルール。トランスポート ルールとも呼ばれる) では、メッセージに最大 10 個の転送受信者を追加できます。詳細については、[ジャーナル、トランスポート、および受信トレイのルールの制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="123c4-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="123c4-p102">受信トレイのルールは、代替ジャーナリング メールボックスでは機能しません。代替ジャーナリング メールボックスの詳細については、[代替ジャーナリング メールボックス](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="123c4-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="123c4-109">これらの問題を修正するには、「[KB 2829319](https://support.microsoft.com/kb/2829319)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="123c4-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="123c4-110">以前の問題が該当しない場合は、Microsoft サポートに問題をエスカレーションする前に、受信トレイのルールの診断レポートを実行します。</span><span class="sxs-lookup"><span data-stu-id="123c4-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="123c4-111">Outlook on the web でメールボックスを開き、**[設定]**、**[オプション]**、**[メールの整理]**、**[受信トレイのルール]** の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="123c4-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="123c4-112">ページの下部にある **[ルールが正しく機能しない場合は、ここをクリックして診断レポートを生成してください]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="123c4-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>

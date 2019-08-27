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
ms.openlocfilehash: 901237d4dc7b99695097142c61a4bfef7c09750d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36555778"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="83e69-102">受信トレイのルールが期待どおりに機能しません</span><span class="sxs-lookup"><span data-stu-id="83e69-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="83e69-103">Outlook on the web で次の設定を確認する:</span><span class="sxs-lookup"><span data-stu-id="83e69-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="83e69-p101">メッセージは、自動的に受信トレイのルールに 1 回だけ従うように、リダイレクト、転送、または返信できます。リダイレクト ルール (受信トレイのルールまたはメール フロー ルール。トランスポート ルールとも呼ばれる) では、メッセージに最大 10 個の転送受信者を追加できます。詳細については、[ジャーナル、トランスポート、および受信トレイのルールの制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="83e69-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="83e69-p102">受信トレイのルールは、代替ジャーナリング メールボックスでは機能しません。代替ジャーナリング メールボックスの詳細については、[代替ジャーナリング メールボックス](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="83e69-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="83e69-109">これらの問題を修正するには、「[KB 2829319](https://support.microsoft.com/kb/2829319)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83e69-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="83e69-110">以前の問題が該当しない場合は、Microsoft サポートに問題をエスカレーションする前に、受信トレイのルールの診断レポートを実行します。</span><span class="sxs-lookup"><span data-stu-id="83e69-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="83e69-111">Outlook on the web でメールボックスを開いて、</span><span class="sxs-lookup"><span data-stu-id="83e69-111">Open the mailbox in Outlook on the web, and click SettingsOptionsOrganize emailInbox rules.</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="83e69-112">**[設定]** > **[Outlook のすべての設定を表示]** > **[メール]** > **[ルール]** の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="83e69-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="83e69-113">ページの下部にある **[ルールが正しく機能しない場合は、ここをクリックして診断レポートを生成してください]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="83e69-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>

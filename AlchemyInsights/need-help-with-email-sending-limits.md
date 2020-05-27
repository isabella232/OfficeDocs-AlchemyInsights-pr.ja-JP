---
title: メールの送信制限についてサポートが必要ですか ?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358728"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="7e4f0-102">メールの送信制限についてサポートが必要ですか ?</span><span class="sxs-lookup"><span data-stu-id="7e4f0-102">Need help with email sending limits?</span></span>

<span data-ttu-id="7e4f0-103">以下では、サービスで適用される **意図的な送信制限**です。</span><span class="sxs-lookup"><span data-stu-id="7e4f0-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="7e4f0-104">これらの制限の詳細については、[ここに](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)記載されています。</span><span class="sxs-lookup"><span data-stu-id="7e4f0-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="7e4f0-105">不要な一括メッセージの配信を防ぐために、**全ての送信メッセージおよび内部メッセージへの受信者の割合制限**をユーザーごとに適用しています。</span><span class="sxs-lookup"><span data-stu-id="7e4f0-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="7e4f0-106">すべての SKU で、この制限は**1 日につき 1 万人の受信者**です。</span><span class="sxs-lookup"><span data-stu-id="7e4f0-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="7e4f0-107">正当な一括商業目的のメッセージ (たとえば、顧客向けのニュースレター) を送信する必要があるカスタマーには、これらのサービスに特化したサード パーティ プロバイダーを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7e4f0-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="7e4f0-108">**注意** 受信者数の制限に達すると、過去 24 時間以内にメッセージを送信した受信者の数が制限を下回るまでメールボックスからメッセージを送信できなくなります。</span><span class="sxs-lookup"><span data-stu-id="7e4f0-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="7e4f0-109">ユーザーは、それまでにメッセージを送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="7e4f0-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="7e4f0-110">**１分あたりに30個のメッセージ**のメッセージ制限が、すべての SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7e4f0-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="7e4f0-111">指定した期間内にユーザーが Exchange Online アカウントから送信できるメッセージの数を決定します。</span><span class="sxs-lookup"><span data-stu-id="7e4f0-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="7e4f0-112">すべての SKU で、1つのメールメッセージに対して、**[宛先]、[Cc]、および[ Bcc] の各フィールドに指定できる受信者の最大数**は、**1000 人の受信者**です。</span><span class="sxs-lookup"><span data-stu-id="7e4f0-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="7e4f0-113">この制限をカスタマイズするには、[ここ](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)に移動します。</span><span class="sxs-lookup"><span data-stu-id="7e4f0-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>

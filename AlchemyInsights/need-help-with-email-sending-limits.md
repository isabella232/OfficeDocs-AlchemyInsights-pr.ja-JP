---
title: メールの送信制限についてサポートが必要ですか ?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: a13eec5d0d1abccd748653e7d7d9bb999b2e3b7a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58328831"
---
# <a name="need-help-with-email-sending-limits"></a>メールの送信制限についてサポートが必要ですか ?

以下では、サービスで適用される **意図的な送信制限** です。 これらの制限の詳細については、[ここに](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)記載されています。

- 不要な一括メッセージの配信を防ぐために、**全ての送信メッセージおよび内部メッセージへの受信者の割合制限** をユーザーごとに適用しています。 すべての SKU で、この制限は **1 日につき 1 万人の受信者** です。  正当な一括商業目的のメッセージ (たとえば、顧客向けのニュースレター) を送信する必要があるカスタマーには、これらのサービスに特化したサード パーティ プロバイダーを使用する必要があります。
    **注意** 受信者数の制限に達すると、過去 24 時間以内にメッセージを送信した受信者の数が制限を下回るまでメールボックスからメッセージを送信できなくなります。 ユーザーは、それまでにメッセージを送信することはできません。
- **１分あたりに30個のメッセージ** のメッセージ制限が、すべての SKU に適用されます。 指定した期間内にユーザーが Exchange Online アカウントから送信できるメッセージの数を決定します。
- すべての SKU で、1 つのメール メッセージに対して、**[宛先]、[Cc]、および [Bcc] の各フィールドに指定できる受信者の最大数** は、**1000 人の受信者** です。この制限をカスタマイズするには、[こちら](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)にアクセスしてください。

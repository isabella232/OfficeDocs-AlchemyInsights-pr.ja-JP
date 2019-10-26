---
title: スパム対策-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/24/2019
ms.locfileid: "37726871"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>エラーコード5.7.23 のメール配信の問題を修正する

Web 上のパブリックに使用可能な SPF または DNS レコードチェッカーで、自分のドメインの SPF DNS レコードを確認します。

送信メッセージが Office 365 によってスパムとして識別され、[高リスク配信プール](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)を経由してルーティングされていないことを確認します。 高リスク配信プール内のメッセージは SPF チェックに合格しないため、宛先の電子メール組織からは受け付けられません。

問題が解決しない場合は、メールを送信しようとしているメールホストの管理者に連絡する必要がある場合があります。 バウンスメッセージで利用できる詳細な外部エラーをメモしておいてください。  Office 365 のサポートは、さらに支援できない場合があります。
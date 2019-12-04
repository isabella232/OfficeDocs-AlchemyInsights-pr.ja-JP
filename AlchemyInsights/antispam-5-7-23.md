---
title: スパム対策 - 5.7.23
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/24/2019
ms.locfileid: "37726871"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>エラー コード 5.7.23 に関するメール配信の問題を修正する

Web 上で一般公開されている SPF または DNS レコード チェックで、自分のドメインの SPF DNS レコードを確認します。

Office 365 により送信メッセージがスパムとして特定されて、[高リスク配信プール](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)経由でルーティングされなかったことを確認します。 高リスク配信プールのメッセージは SPF チェックに合格しないため、送信先のメール組織によって承認されません。

問題が解決しない場合は、メール送信先のメール ホスト管理者への連絡が必要な場合があります。 バウンス メッセージに表示される詳細な外部エラーをメモします。  Office 365 のサポートでは、これ以上のアシスタントは提供できない可能性があります。
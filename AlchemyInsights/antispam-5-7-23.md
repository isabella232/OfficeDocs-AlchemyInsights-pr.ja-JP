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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676502"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>エラー コード 5.7.23 に関するメール配信の問題を修正する

Web 上で一般公開されている SPF または DNS レコード チェックで、自分のドメインの SPF DNS レコードを確認します。

Microsoft により送信メッセージがスパムとして特定されて、[高リスク配信プール](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)経由でルーティングされなかったことを確認します。 高リスク配信プールのメッセージは SPF チェックに合格しないため、送信先のメール組織によって承認されません。

問題が解決しない場合は、メール送信先のメール ホスト管理者への連絡が必要な場合があります。 バウンス メッセージに表示される詳細な外部エラーをメモします。 Microsoft のサポートでは、これ以上のアシスタントは提供できない可能性があります。

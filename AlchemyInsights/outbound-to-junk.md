---
title: 送信メールが迷惑メール フォルダーへ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 2350586e95f316061ff855d152e86db0547eb209
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761173"
---
# <a name="outbound-email-to-junk-email-folder"></a>送信メールが迷惑メール フォルダーへ

送信メッセージが迷惑メールとしてマークされている場合には、以下の手順を実行します。

- まだ行っていない場合は、[送信スパム ポリシー通知の設定](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy)を検討してください。

- [メッセージ トレース](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc)を使用して、イベント値 **Spam** があるかどうかを確認します。この値は送信メッセージに追加の詳細情報 (**危険度の高い配信プールを使用する**) を含みます。

  これらのメッセージについては、メッセージの内容を確認し、スパムとして考えられる可能性のあるものを確認してください。 たとえば、署名が多くのユーザーに対して問題を引き起こすことがあります。

  迷惑メールとしてマークされている正当な送信メッセージの例が複数ある場合にはサポート チケットを開き、そのメッセージを誤検出としてスパム アナリストに送信するようサポート エージェントに依頼してください。 すべてのメッセージ ヘッダーを含むサンプル メッセージを提供する準備をします。

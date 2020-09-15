---
title: 送信メールが迷惑メール フォルダーへ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769188"
---
# <a name="outbound-email-to-junk-email-folder"></a>送信メールが迷惑メール フォルダーへ

送信メッセージが迷惑メールとしてマークされている場合には、以下の手順を実行します。

- まだ行っていない場合は、[送信スパム ポリシー通知の設定](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)を検討してください。

- [メッセージ トレース](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc)を使用して、イベント値 **Spam** があるかどうかを確認します。この値は送信メッセージに追加の詳細情報 (**危険度の高い配信プールを使用する**) を含みます。

  これらのメッセージについては、メッセージの内容を確認し、スパムとして考えられる可能性のあるものを確認してください。 たとえば、署名が多くのユーザーに対して問題を引き起こすことがあります。

  迷惑メールとしてマークされている正当な送信メッセージの例が複数ある場合にはサポート チケットを開き、そのメッセージを誤検出としてスパム アナリストに送信するようサポート エージェントに依頼してください。 すべてのメッセージ ヘッダーを含むサンプル メッセージを提供する準備をします。

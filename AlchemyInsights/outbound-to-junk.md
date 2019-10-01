---
title: 迷惑メールフォルダーへの送信メール
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 371d2c46e9048365fd343145330536bd9cf1db82
ms.sourcegitcommit: 1002f510fadb92c143cd6bbb60b42a851d5a38e1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/20/2019
ms.locfileid: "37313910"
---
# <a name="outbound-email-to-junk-email-folder"></a>迷惑メールフォルダーへの送信メール

送信メッセージが迷惑メールとしてマークされている場合は、次の手順を実行します。

- まだ[送信スパムポリシー通知の構成](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy)を検討してください。

- [メッセージ追跡](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc)を使用して、送信メッセージに追加の詳細情報を含むイベント値が**スパム**であるかどうかを確認します。 [**高リスク配信プールを使用**する。

  これらのメッセージでは、メッセージの内容をチェックして、スパムと見なされる内容を確認します。 たとえば、署名は多くのユーザーにとって問題を引き起こすことがあります。

  迷惑メールとしてマークされている正当な送信メッセージの例が複数ある場合は、サポートチケットを開いて、メッセージを誤検知としてスパムアナリストに送信するようサポートエージェントに依頼します。 すべてのメッセージヘッダーを含むサンプルメッセージを提供できるように準備します。

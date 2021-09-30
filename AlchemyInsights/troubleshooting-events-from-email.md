---
title: メールからのイベントのトラブルシューティング
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
- "9000301"
- "5765"
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105357"
---
# <a name="troubleshooting-events-from-email"></a>メールからのイベントのトラブルシューティング

1. メールボックスで機能が有効になっていることを確認します: **Get-EventsFromEmailConfiguration -ID <mailbox>**

2. 次に、「メールからのイベント」のログ **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile** を確認します

3. 「メールからのイベント」ログで、メールボックス内のアイテムと一致する InternetMessageId を見つけます。  

4. TrustScore は、アイテムが追加されるかどうかを決定します。 イベントは、TrustScore = "Trusted" の場合にのみ追加されます。

TrustScore は、メッセージ ヘッダーにある SPF、Dkim、または Dmarc プロパティによって決定されます。

これらのプロパティを表示するには:

**デスクトップ版 Outlook**

- アイテムを開く
- ファイル -> プロパティ -> インターネット ヘッダー

または

**MFCMapi**

- 受信トレイのアイテムに移動する
- PR_TRANSPORT_MESSAGE_HEADERS_W を探す

これらのプロパティは、トランスポートおよびルーティング中に決定および記録されます。 詳細なトラブルシューティングを行うには、SPF、DKIM、DMARC での障害についてトランスポート サポートをフォローアップする必要がある場合があります。
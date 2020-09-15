---
title: メールからのイベントのトラブルシューティング
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658739"
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

これらのプロパティは、トランスポートおよびルーティング中に決定および記録されます。 さらにトラブルシューティングを行うには、SPF、DKIM、DMARC での障害についてトランスポート サポートをフォローアップする必要がある場合があります。
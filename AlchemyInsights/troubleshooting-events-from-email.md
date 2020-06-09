---
title: メールからのイベントのトラブルシューティング
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569865"
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
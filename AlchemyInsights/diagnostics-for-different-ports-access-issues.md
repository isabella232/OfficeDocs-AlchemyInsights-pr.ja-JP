---
title: さまざまなポート アクセスの問題の診断
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030907"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>さまざまなポート アクセスの問題の診断

さまざまなポート アクセスの問題を解決するには、次の手順を実行します。

1. ポータルから仮想マシン (VM) を停止/割り当て解除し、VM を再起動して、再度テストします。 
2. VM のネットワーク設定を確認して、トラフィックをブロックしているネットワーク セキュリティ グループ (NSG) があるかどうかを確認します。 [Network Watcher の IP フロー検証ツール](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support)を使用して、トラフィックをブロックしている NSG、オンプレミス（「デフォルトルート」0.0.0.0/0）、またはネットワーク アプライアンスにトラフィックを再ルーティングするユーザー定義ルート (UDR) を確認することもできます。
上記の手順を試しても問題が解決しない場合は、さらに診断するために、メールを送信しようとしている VM 名と TCP ポートを入力してください。

**おすすめのドキュメント**

[ポート 25 を介して送信メールを送信するための制限と推奨事項](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)
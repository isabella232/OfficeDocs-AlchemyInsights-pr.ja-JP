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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038232"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>さまざまなポート アクセスの問題の診断

さまざまなポート アクセスの問題を解決するには、次の手順を実行します。

1. ポータルから仮想マシン (VM) を停止/割り当て解除し、VM を再起動して、再度テストします。 
2. VM のネットワーク設定を確認して、トラフィックをブロックしているネットワーク セキュリティ グループ (NSG) があるかどうかを確認します。 [Network Watcher の IP フロー検証ツール](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support)を使用して、トラフィックをブロックしている NSG、オンプレミス（「デフォルトルート」0.0.0.0/0）、またはネットワーク アプライアンスにトラフィックを再ルーティングするユーザー定義ルート (UDR) を確認することもできます。
上記の手順を試しても問題が解決しない場合は、さらに診断するために、メールを送信しようとしている VM 名と TCP ポートを入力してください。

**おすすめのドキュメント**

[ポート 25 を介して送信メールを送信するための制限と推奨事項](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)
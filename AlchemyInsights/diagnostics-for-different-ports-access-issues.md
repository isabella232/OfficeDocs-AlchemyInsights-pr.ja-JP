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
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="e8cc9-102">さまざまなポート アクセスの問題の診断</span><span class="sxs-lookup"><span data-stu-id="e8cc9-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="e8cc9-103">さまざまなポート アクセスの問題を解決するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="e8cc9-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="e8cc9-104">ポータルから仮想マシン (VM) を停止/割り当て解除し、VM を再起動して、再度テストします。</span><span class="sxs-lookup"><span data-stu-id="e8cc9-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="e8cc9-105">VM のネットワーク設定を確認して、トラフィックをブロックしているネットワーク セキュリティ グループ (NSG) があるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="e8cc9-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="e8cc9-106">[Network Watcher の IP フロー検証ツール](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support)を使用して、トラフィックをブロックしている NSG、オンプレミス（「デフォルトルート」0.0.0.0/0）、またはネットワーク アプライアンスにトラフィックを再ルーティングするユーザー定義ルート (UDR) を確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="e8cc9-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="e8cc9-107">上記の手順を試しても問題が解決しない場合は、さらに診断するために、メールを送信しようとしている VM 名と TCP ポートを入力してください。</span><span class="sxs-lookup"><span data-stu-id="e8cc9-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="e8cc9-108">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="e8cc9-108">**Recommended Documents**</span></span>

[<span data-ttu-id="e8cc9-109">ポート 25 を介して送信メールを送信するための制限と推奨事項</span><span class="sxs-lookup"><span data-stu-id="e8cc9-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)
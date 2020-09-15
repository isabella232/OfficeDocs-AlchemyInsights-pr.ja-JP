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
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="9b9c6-102">メールからのイベントのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="9b9c6-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="9b9c6-103">メールボックスで機能が有効になっていることを確認します: **Get-EventsFromEmailConfiguration -ID <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="9b9c6-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="9b9c6-104">次に、「メールからのイベント」のログ **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile** を確認します</span><span class="sxs-lookup"><span data-stu-id="9b9c6-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="9b9c6-105">「メールからのイベント」ログで、メールボックス内のアイテムと一致する InternetMessageId を見つけます。</span><span class="sxs-lookup"><span data-stu-id="9b9c6-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="9b9c6-106">TrustScore は、アイテムが追加されるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="9b9c6-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="9b9c6-107">イベントは、TrustScore = "Trusted" の場合にのみ追加されます。</span><span class="sxs-lookup"><span data-stu-id="9b9c6-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="9b9c6-108">TrustScore は、メッセージ ヘッダーにある SPF、Dkim、または Dmarc プロパティによって決定されます。</span><span class="sxs-lookup"><span data-stu-id="9b9c6-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="9b9c6-109">これらのプロパティを表示するには:</span><span class="sxs-lookup"><span data-stu-id="9b9c6-109">To view these properties:</span></span>

<span data-ttu-id="9b9c6-110">**デスクトップ版 Outlook**</span><span class="sxs-lookup"><span data-stu-id="9b9c6-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="9b9c6-111">アイテムを開く</span><span class="sxs-lookup"><span data-stu-id="9b9c6-111">Open the item</span></span>
- <span data-ttu-id="9b9c6-112">ファイル -> プロパティ -> インターネット ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b9c6-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="9b9c6-113">または</span><span class="sxs-lookup"><span data-stu-id="9b9c6-113">or</span></span>

<span data-ttu-id="9b9c6-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="9b9c6-114">**MFCMapi**</span></span>

- <span data-ttu-id="9b9c6-115">受信トレイのアイテムに移動する</span><span class="sxs-lookup"><span data-stu-id="9b9c6-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="9b9c6-116">PR_TRANSPORT_MESSAGE_HEADERS_W を探す</span><span class="sxs-lookup"><span data-stu-id="9b9c6-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="9b9c6-117">これらのプロパティは、トランスポートおよびルーティング中に決定および記録されます。</span><span class="sxs-lookup"><span data-stu-id="9b9c6-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="9b9c6-118">さらにトラブルシューティングを行うには、SPF、DKIM、DMARC での障害についてトランスポート サポートをフォローアップする必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="9b9c6-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>
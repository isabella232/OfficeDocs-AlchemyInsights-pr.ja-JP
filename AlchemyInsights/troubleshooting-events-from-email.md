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
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834844"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="36954-102">メールからのイベントのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="36954-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="36954-103">メールボックスで機能が有効になっていることを確認します: **Get-EventsFromEmailConfiguration -ID <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="36954-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="36954-104">次に、「メールからのイベント」のログ **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile** を確認します</span><span class="sxs-lookup"><span data-stu-id="36954-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="36954-105">「メールからのイベント」ログで、メールボックス内のアイテムと一致する InternetMessageId を見つけます。</span><span class="sxs-lookup"><span data-stu-id="36954-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="36954-106">TrustScore は、アイテムが追加されるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="36954-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="36954-107">イベントは、TrustScore = "Trusted" の場合にのみ追加されます。</span><span class="sxs-lookup"><span data-stu-id="36954-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="36954-108">TrustScore は、メッセージ ヘッダーにある SPF、Dkim、または Dmarc プロパティによって決定されます。</span><span class="sxs-lookup"><span data-stu-id="36954-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="36954-109">これらのプロパティを表示するには:</span><span class="sxs-lookup"><span data-stu-id="36954-109">To view these properties:</span></span>

<span data-ttu-id="36954-110">**デスクトップ版 Outlook**</span><span class="sxs-lookup"><span data-stu-id="36954-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="36954-111">アイテムを開く</span><span class="sxs-lookup"><span data-stu-id="36954-111">Open the item</span></span>
- <span data-ttu-id="36954-112">ファイル -> プロパティ -> インターネット ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36954-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="36954-113">または</span><span class="sxs-lookup"><span data-stu-id="36954-113">or</span></span>

<span data-ttu-id="36954-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="36954-114">**MFCMapi**</span></span>

- <span data-ttu-id="36954-115">受信トレイのアイテムに移動する</span><span class="sxs-lookup"><span data-stu-id="36954-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="36954-116">PR_TRANSPORT_MESSAGE_HEADERS_W を探す</span><span class="sxs-lookup"><span data-stu-id="36954-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="36954-117">これらのプロパティは、トランスポートおよびルーティング中に決定および記録されます。</span><span class="sxs-lookup"><span data-stu-id="36954-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="36954-118">さらにトラブルシューティングを行うには、SPF、DKIM、DMARC での障害についてトランスポート サポートをフォローアップする必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="36954-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>
---
title: パブリック フォルダーの移行バッチが完了せず、同期が表示される
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 33302110249b02aef87639792ebfd9cafd6638c0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47804427"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="d96e7-102">パブリック フォルダーの移行バッチが完了せず、同期が表示される</span><span class="sxs-lookup"><span data-stu-id="d96e7-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="d96e7-103">移行バッチの完了を開始した可能性があり、移行バッチの状態が非常に長い間 [同期済み] と表示され続けます。</span><span class="sxs-lookup"><span data-stu-id="d96e7-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="d96e7-104">これは想定された動作です。</span><span class="sxs-lookup"><span data-stu-id="d96e7-104">This is expected behavior.</span></span>

<span data-ttu-id="d96e7-105">移行バッチの状態は、[完了] に切り替わる前に数時間 [同期済み] のままになるのが一般的です。</span><span class="sxs-lookup"><span data-stu-id="d96e7-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="d96e7-106">多数のターゲット メールボックスを含む移行の場合、基になるパブリック フォルダーの移行の要求が失敗または検疫されていない限り、状態は 24 時間以上 [同期済み] 状態のままです。</span><span class="sxs-lookup"><span data-stu-id="d96e7-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="d96e7-107">移行バッチがタスクを完了するまでに 24 - 48 時間かかります。</span><span class="sxs-lookup"><span data-stu-id="d96e7-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

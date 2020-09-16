---
title: CompletedWithErrors 状態のパブリック フォルダー移行バッチについて
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744118"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="23b80-102">CompletedWithErrors 状態のパブリック フォルダー移行バッチについて</span><span class="sxs-lookup"><span data-stu-id="23b80-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="23b80-103">次の手順を使用してバッチを完了し、大きなアイテムまたは不良アイテムをスキップします。</span><span class="sxs-lookup"><span data-stu-id="23b80-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="23b80-104">移行バッチで、スキップされたアイテムを承認します。</span><span class="sxs-lookup"><span data-stu-id="23b80-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="23b80-105">次のコマンドを使用して、“同期済み” でも完了していない、移行要求でスキップされたアイテムを承認します。</span><span class="sxs-lookup"><span data-stu-id="23b80-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="23b80-106">移行バッチおよび要求は再開され、数分で完了します。</span><span class="sxs-lookup"><span data-stu-id="23b80-106">The migration batch and requests should resume and complete in a few minutes.</span></span>


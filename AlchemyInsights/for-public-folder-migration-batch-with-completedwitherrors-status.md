---
title: CompletedWithErrors 状態のパブリック フォルダー移行バッチについて
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158616"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="3b033-102">CompletedWithErrors 状態のパブリック フォルダー移行バッチについて</span><span class="sxs-lookup"><span data-stu-id="3b033-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="3b033-103">次の手順を使用してバッチを完了し、大きなアイテムまたは不良アイテムをスキップします。</span><span class="sxs-lookup"><span data-stu-id="3b033-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="3b033-104">移行バッチで、スキップされたアイテムを承認します。</span><span class="sxs-lookup"><span data-stu-id="3b033-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="3b033-105">次のコマンドを使用して、“同期済み” でも完了していない、移行要求でスキップされたアイテムを承認します。</span><span class="sxs-lookup"><span data-stu-id="3b033-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="3b033-106">移行バッチおよび要求は再開され、数分で完了します。</span><span class="sxs-lookup"><span data-stu-id="3b033-106">The migration batch and requests should resume and complete in a few minutes.</span></span>


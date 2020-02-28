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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>CompletedWithErrors 状態のパブリック フォルダー移行バッチについて

次の手順を使用してバッチを完了し、大きなアイテムまたは不良アイテムをスキップします。 
1. 移行バッチで、スキップされたアイテムを承認します。

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. 次のコマンドを使用して、“同期済み” でも完了していない、移行要求でスキップされたアイテムを承認します。

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. 移行バッチおよび要求は再開され、数分で完了します。


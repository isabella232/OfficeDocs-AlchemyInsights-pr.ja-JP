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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744118"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>CompletedWithErrors 状態のパブリック フォルダー移行バッチについて

次の手順を使用してバッチを完了し、大きなアイテムまたは不良アイテムをスキップします。 
1. 移行バッチで、スキップされたアイテムを承認します。

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. 次のコマンドを使用して、“同期済み” でも完了していない、移行要求でスキップされたアイテムを承認します。

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. 移行バッチおよび要求は再開され、数分で完了します。


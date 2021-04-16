---
title: CompletedWithErrors 状態のパブリック フォルダー移行バッチについて
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812469"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>CompletedWithErrors 状態のパブリック フォルダー移行バッチについて

次の手順を使用してバッチを完了し、大きなアイテムまたは不良アイテムをスキップします。 
1. 移行バッチで、スキップされたアイテムを承認します。

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. 次のコマンドを使用して、“同期済み” でも完了していない、移行要求でスキップされたアイテムを承認します。

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. 移行バッチおよび要求は再開され、数分で完了します。


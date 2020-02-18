---
title: CompletedWithErrors status を使用したパブリックフォルダーの移行バッチの場合
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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2020
ms.locfileid: "42094387"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>CompletedWithErrors status を使用したパブリックフォルダーの移行バッチの場合

次の手順を使用してバッチを完了し、大きい/不良アイテムをスキップします。 
1. 移行バッチでスキップされたアイテムを承認します。

    New-migrationbatch \<batchname>-ApproveSkippedItems 
2. 次のコマンドを使用して、"同期されましたが完了していません" という移行要求でスキップされたアイテムを承認します。

    $pf = Remove-publicfoldermailboxmigrationrequest |Get-publicfoldermailboxmigrationrequeststatistics-IncludeReport;ForEach ($i $pf) {if $i () {if (LargeItemsEncountered-gt 0-$i or BadItemsEncountered-gt 0) {Remove-publicfoldermailboxmigrationrequest $i UtcNow-SkippedItemApprovalTime $ ([DateTime]::)}}}}
3. 移行バッチと要求は、数分で再開して完了する必要があります。


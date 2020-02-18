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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="79e66-102">CompletedWithErrors status を使用したパブリックフォルダーの移行バッチの場合</span><span class="sxs-lookup"><span data-stu-id="79e66-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="79e66-103">次の手順を使用してバッチを完了し、大きい/不良アイテムをスキップします。</span><span class="sxs-lookup"><span data-stu-id="79e66-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="79e66-104">移行バッチでスキップされたアイテムを承認します。</span><span class="sxs-lookup"><span data-stu-id="79e66-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="79e66-105">New-migrationbatch \<batchname>-ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="79e66-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="79e66-106">次のコマンドを使用して、"同期されましたが完了していません" という移行要求でスキップされたアイテムを承認します。</span><span class="sxs-lookup"><span data-stu-id="79e66-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="79e66-107">$pf = Remove-publicfoldermailboxmigrationrequest |Get-publicfoldermailboxmigrationrequeststatistics-IncludeReport;ForEach ($i $pf) {if $i () {if (LargeItemsEncountered-gt 0-$i or BadItemsEncountered-gt 0) {Remove-publicfoldermailboxmigrationrequest $i UtcNow-SkippedItemApprovalTime $ ([DateTime]::)}}}}</span><span class="sxs-lookup"><span data-stu-id="79e66-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="79e66-108">移行バッチと要求は、数分で再開して完了する必要があります。</span><span class="sxs-lookup"><span data-stu-id="79e66-108">The migration batch and requests should resume and complete in a few minutes.</span></span>


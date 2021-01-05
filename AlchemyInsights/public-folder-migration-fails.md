---
title: パブリック フォルダーの移行が 95% で失敗する
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
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804399"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="8cae8-102">パブリック フォルダーの移行が 95% で失敗する</span><span class="sxs-lookup"><span data-stu-id="8cae8-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="8cae8-103">移行バッチの完了を開始した可能性があり、移行バッチの状態が非常に長い間 [**同期済み**] と表示され続けます。</span><span class="sxs-lookup"><span data-stu-id="8cae8-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="8cae8-104">これは想定された動作です。</span><span class="sxs-lookup"><span data-stu-id="8cae8-104">This is expected behavior.</span></span>

<span data-ttu-id="8cae8-105">移行バッチの状態は、[**完了**] に切り替わる前に数時間 [**同期済み**] のままになるのが一般的です。</span><span class="sxs-lookup"><span data-stu-id="8cae8-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="8cae8-106">多数のターゲット メールボックスを含む移行の場合、基になるパブリック フォルダーの移行の要求が失敗または検疫されていない限り、状態は 24 時間以上 [同期済み] 状態のままです。</span><span class="sxs-lookup"><span data-stu-id="8cae8-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="8cae8-107">移行バッチがタスクを完了するまでに 24 - 48 時間かかります。</span><span class="sxs-lookup"><span data-stu-id="8cae8-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="8cae8-108">パブリック フォルダーの移行が 95% で失敗し、エラー FailedToMailEnablePublicFoldersException が発生する場合:</span><span class="sxs-lookup"><span data-stu-id="8cae8-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="8cae8-109">Exchange オンプレミス サーバーで [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) スクリプトをダウンロードして実行します。</span><span class="sxs-lookup"><span data-stu-id="8cae8-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="8cae8-110">スクリプトによって提案された修正操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="8cae8-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="8cae8-111">Sync-MailPublicFolders (Exchange 2010 の場合) または Sync-ModernMailPublicFolders (Exchange 2013 以降の場合) を実行します。</span><span class="sxs-lookup"><span data-stu-id="8cae8-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="8cae8-112">パブリック フォルダーの移行を開始します。</span><span class="sxs-lookup"><span data-stu-id="8cae8-112">Resume public folder migration.</span></span>

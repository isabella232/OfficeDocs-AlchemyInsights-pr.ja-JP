---
title: 共有リンクのダウンロードを禁止する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358747"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="9e5b9-102">共有リンクのダウンロードを禁止する</span><span class="sxs-lookup"><span data-stu-id="9e5b9-102">Block download on sharing links</span></span>

<span data-ttu-id="9e5b9-103">Office ドキュメントの**表示専用リンク**に対し、**ダウンロードの禁止**を設定できます。</span><span class="sxs-lookup"><span data-stu-id="9e5b9-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="9e5b9-104">このオプションを選択すると、作成したリンクを介してファイルにアクセスできるユーザーに、ファイルをダウンロード、印刷、またはコピーするオプションが表示されません。</span><span class="sxs-lookup"><span data-stu-id="9e5b9-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="9e5b9-105">管理者は、[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps)または[Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell コマンドレットの `BlockDownloadLinksFileType` 設定を変更することで、Office ファイルに対してのみ「ダウンロード禁止」設定を表示するかどうかを制御できます。</span><span class="sxs-lookup"><span data-stu-id="9e5b9-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>

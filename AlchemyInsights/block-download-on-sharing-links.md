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
# <a name="block-download-on-sharing-links"></a>共有リンクのダウンロードを禁止する

Office ドキュメントの**表示専用リンク**に対し、**ダウンロードの禁止**を設定できます。 このオプションを選択すると、作成したリンクを介してファイルにアクセスできるユーザーに、ファイルをダウンロード、印刷、またはコピーするオプションが表示されません。

管理者は、[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps)または[Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell コマンドレットの `BlockDownloadLinksFileType` 設定を変更することで、Office ファイルに対してのみ「ダウンロード禁止」設定を表示するかどうかを制御できます。

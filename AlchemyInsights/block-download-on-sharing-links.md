---
title: 共有リンクのダウンロードを禁止する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685747"
---
# <a name="block-download-on-sharing-links"></a>共有リンクのダウンロードを禁止する

Office ドキュメントの**表示専用リンク**に対し、**ダウンロードの禁止**を設定できます。 このオプションを選択すると、作成したリンクを介してファイルにアクセスできるユーザーに、ファイルをダウンロード、印刷、またはコピーするオプションが表示されません。

管理者は、[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps)または[Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell コマンドレットの `BlockDownloadLinksFileType` 設定を変更することで、Office ファイルに対してのみ「ダウンロード禁止」設定を表示するかどうかを制御できます。

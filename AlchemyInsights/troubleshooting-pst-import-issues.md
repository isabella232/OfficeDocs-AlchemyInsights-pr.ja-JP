---
title: PST インポートに関する問題のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826168"
---
# <a name="troubleshooting-pst-import-issues"></a>PST インポートに関する問題のトラブルシューティング

- Outlook クライアント自体でインポートしている場合は、「[Outlook .pst ファイルにインポートするときの問題を解決する](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)」を参照してください。

- インポート サービスを使用していて、それがスタックしている場合、Azure Storage の場所にアップロードするそれぞれの PST ファイルは 20 GB 以下である必要があります。 PST ファイルが 20 GB を超える場合、PST インポート プロセスのパフォーマンスに影響を与える場合があります。

- 特定のインポート ジョブの状態を確認したい場合、[Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest) を使用することができます。

- インポート サービスの詳細については、「[組織の PST ファイルのインポートの概要](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)」を参照してください。

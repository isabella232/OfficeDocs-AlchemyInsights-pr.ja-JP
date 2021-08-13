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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972424"
---
# <a name="troubleshooting-pst-import-issues"></a>PST インポートに関する問題のトラブルシューティング

- Outlook クライアント自体でインポートしている場合は、「[Outlook .pst ファイルにインポートするときの問題を解決する](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)」を参照してください。

- インポート サービスを使用していて、それがスタックしている場合、Azure Storage の場所にアップロードするそれぞれの PST ファイルは 20 GB 以下である必要があります。 PST ファイルが 20 GB を超える場合、PST インポート プロセスのパフォーマンスに影響を与える場合があります。 スタックしたジョブのトラブルシューティングに関する詳細については、「[Issues that affect PST import jobs (PST インポート ジョブに影響を与える問題)](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)」を参照してください。

- 特定のインポート ジョブの状態を確認する場合は、[Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest) を使用してください。

- インポート サービスに関する詳細については、「[組織の PST ファイルのインポートの概要](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)」を参照してください。

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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059820"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="3bc1a-102">PST インポートに関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="3bc1a-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="3bc1a-103">Outlook クライアント自体でインポートしている場合は、「[Outlook .pst ファイルにインポートするときの問題を解決する](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bc1a-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="3bc1a-104">インポート サービスを使用していて、それがスタックしている場合、Azure Storage の場所にアップロードするそれぞれの PST ファイルは 20 GB 以下である必要があります。</span><span class="sxs-lookup"><span data-stu-id="3bc1a-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="3bc1a-105">PST ファイルが 20 GB を超える場合、PST インポート プロセスのパフォーマンスに影響を与える場合があります。</span><span class="sxs-lookup"><span data-stu-id="3bc1a-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="3bc1a-106">スタックしたジョブのトラブルシューティングに関する詳細については、「[Issues that affect PST import jobs (PST インポート ジョブに影響を与える問題)](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bc1a-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="3bc1a-107">特定のインポート ジョブの状態を確認する場合は、[Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest) を使用してください。</span><span class="sxs-lookup"><span data-stu-id="3bc1a-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="3bc1a-108">インポート サービスに関する詳細については、「[組織の PST ファイルのインポートの概要](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bc1a-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>

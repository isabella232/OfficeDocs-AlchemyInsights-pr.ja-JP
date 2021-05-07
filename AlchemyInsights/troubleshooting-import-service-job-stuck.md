---
title: インポート サービス ジョブがスタックしたときのトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125840"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="b80aa-102">インポート サービス ジョブがスタックしたときのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="b80aa-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="b80aa-103">インポート サービス ジョブがスタックまたは失敗する問題が発生している場合は、以下を調べて試してください。</span><span class="sxs-lookup"><span data-stu-id="b80aa-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="b80aa-104">PST ファイルのサイズを確認します。</span><span class="sxs-lookup"><span data-stu-id="b80aa-104">Review the size of of the PST file.</span></span> <span data-ttu-id="b80aa-105">インポート用の PST ファイルの最大推奨サイズは 20 GB です。</span><span class="sxs-lookup"><span data-stu-id="b80aa-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="b80aa-106">破損が原因でスキップされたアイテムが疑われる場合は、Scanpst.exe を実行して、PST ファイルのエラーを診断および修正してください。</span><span class="sxs-lookup"><span data-stu-id="b80aa-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="b80aa-107">インポート中に「MapiExceptionShutoffQuotaExceeded」エラーが表示された場合は、ターゲット メールボックスに目的の PST ファイルをインポートするのに十分な容量があることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b80aa-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="b80aa-108">PST インポート ジョブの問題のトラブルシューティングの詳細については、「[Troubleshoot issues with PST import jobs (PST インポート ジョブの問題のトラブルシューティング)](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b80aa-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="b80aa-109">PST を Outlook にインポートする際の問題を修正する方法については、「[Fix problems importing an Outlook .pst file (microsoft.com) (Outlook .pst ファイル (microsoft.com) のインポートに関する問題を修正する)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b80aa-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>
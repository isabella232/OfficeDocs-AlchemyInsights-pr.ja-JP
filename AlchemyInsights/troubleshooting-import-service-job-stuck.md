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
ms.openlocfilehash: bf07102d01d85eaed8ea95b571a0eabea7c4b7448839294f37e5e30134e04282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105105"
---
# <a name="troubleshooting-import-service-job-stuck"></a>インポート サービス ジョブがスタックしたときのトラブルシューティング

インポート サービス ジョブがスタックまたは失敗する問題が発生している場合は、以下を調べて試してください。

- PST ファイルのサイズを確認します。 インポート用の PST ファイルの最大推奨サイズは 20 GB です。

- 破損が原因でスキップされたアイテムが疑われる場合は、Scanpst.exe を実行して、PST ファイルのエラーを診断および修正してください。

- インポート中に「MapiExceptionShutoffQuotaExceeded」エラーが表示された場合は、ターゲット メールボックスに目的の PST ファイルをインポートするのに十分な容量があることを確認してください。

PST インポート ジョブの問題のトラブルシューティングの詳細については、「[Troubleshoot issues with PST import jobs (PST インポート ジョブの問題のトラブルシューティング)](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)」を参照してください。

PST を Outlook にインポートする際の問題を修正する方法については、「[Fix problems importing an Outlook .pst file (microsoft.com) (Outlook .pst ファイル (microsoft.com) のインポートに関する問題を修正する)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)」を参照してください。
---
title: Microsoft Defender for Endpoints へのマシンのオンボードに関する問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901572"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="bd33c-102">Microsoft Defender for Endpoints へのマシンのオンボードに関する問題</span><span class="sxs-lookup"><span data-stu-id="bd33c-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="bd33c-103">MDE サービスへのマシンのオンボードに問題がある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="bd33c-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="bd33c-104">エンド ユーザーのマシンにアクセスできる場合は、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="bd33c-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="bd33c-105">[MDE クライアント アナライザー](https://aka.ms/betamdeanalyzer)診断ツールの最新のプレビュー バージョンをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="bd33c-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="bd33c-106">**MDEClientAnalyzer.cmd** を右クリックし、[管理者として実行] を選択します。</span><span class="sxs-lookup"><span data-stu-id="bd33c-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="bd33c-107">**MDEClientAnalyzer.htm** で提案されているガイダンスに従ってください。</span><span class="sxs-lookup"><span data-stu-id="bd33c-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="bd33c-108">より詳細なログについては、**MDEClientAnalyzerResult** という名前の作成されたサブフォルダーを確認してください。</span><span class="sxs-lookup"><span data-stu-id="bd33c-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="bd33c-109">追加のガイダンスが必要な場合は、[Microsoft Defender for Endpoint のサポート](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support)に連絡し、分析のために結果の MDEClientAnalyzerResult.zip ファイルを提供してください。</span><span class="sxs-lookup"><span data-stu-id="bd33c-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>

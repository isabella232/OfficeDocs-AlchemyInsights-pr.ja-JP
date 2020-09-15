---
title: マシンのオンボードの問題
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
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676887"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="f924b-102">マシンのオンボードの問題</span><span class="sxs-lookup"><span data-stu-id="f924b-102">Issues with onboarding machines</span></span>

<span data-ttu-id="f924b-103">MDATP サービスへのマシンのオンボードに問題がある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f924b-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="f924b-104">エンド ユーザーのマシンにアクセスできる場合は、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="f924b-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="f924b-105">[クライアント接続アナライザー](https://aka.ms/mdatpanalyzer)の診断ツールをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="f924b-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="f924b-106">展開し、MDATPAnalyzer.cmd を実行します。</span><span class="sxs-lookup"><span data-stu-id="f924b-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="f924b-107">MDATPClientAnalyzerResult というフォルダーにある診断ログを見つけます。これは、アナライザー ツールがダウンロードされたフォルダーと同じです。</span><span class="sxs-lookup"><span data-stu-id="f924b-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="f924b-108">ログ ファイル (MDATPClientAnalyzer.txt) を確認して、接続またはインターネット プロキシ設定の問題を見つけます。</span><span class="sxs-lookup"><span data-stu-id="f924b-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>
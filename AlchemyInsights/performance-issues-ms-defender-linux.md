---
title: Linux 用 Microsoft Defender for Endpoint のパフォーマンスの問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794270"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="efcdd-102">Linux 用 Microsoft Defender for Endpoint のパフォーマンスの問題</span><span class="sxs-lookup"><span data-stu-id="efcdd-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="efcdd-103">この記事では、Linux 上の Microsoft Defender for Endpoint のパフォーマンスの問題を特定する手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="efcdd-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="efcdd-104">最初に、発生している問題が[最新バージョン](/microsoft-365/security/defender-endpoint/linux-whatsnew)で解決されていることを確認することが重要です。</span><span class="sxs-lookup"><span data-stu-id="efcdd-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="efcdd-105">調査を開始するには、「[Linux用の Microsoft Defender for Endpoint のパフォーマンスの問題のトラブルシューティング](/microsoft-365/security/defender-endpoint/linux-support-perf)」 を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efcdd-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="efcdd-106">除外</span><span class="sxs-lookup"><span data-stu-id="efcdd-106">Exclusions</span></span>

<span data-ttu-id="efcdd-107">除外は、パフォーマンスの問題を軽減するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="efcdd-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="efcdd-108">開始する前に除外をレビューし、追加のリスクが認識されて文書化されるようにします。</span><span class="sxs-lookup"><span data-stu-id="efcdd-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="efcdd-109">詳細については、「[Linux 用の Microsoft Defender for Endpoint の除外を構成および検証する](/microsoft-365/security/defender-endpoint/linux-exclusions)」 を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efcdd-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="efcdd-110">除外するファイルとフォルダーが複数あり、それらがすべて同じマウント ポイントにある場合は、マウントポイントを除外する方が簡単な場合があります。</span><span class="sxs-lookup"><span data-stu-id="efcdd-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="efcdd-111">2 月のリリース 101.22.80 以降では、マウントポイント全体を除外できます。</span><span class="sxs-lookup"><span data-stu-id="efcdd-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="efcdd-112">たとえば、/mnt/backup がマウントポイントの場合は、次のコマンドを実行して除外リストに /mnt/backup を追加できます。</span><span class="sxs-lookup"><span data-stu-id="efcdd-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="efcdd-113">**注**: 除外を追加すると、マルウェアが検出されないリスクが高まるので、慎重に処理して実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="efcdd-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="efcdd-114">お困りですか?</span><span class="sxs-lookup"><span data-stu-id="efcdd-114">Need Help?</span></span>

<span data-ttu-id="efcdd-115">最も効率的な方法で支援するには、サポート ケースを開く前に診断データを収集します。</span><span class="sxs-lookup"><span data-stu-id="efcdd-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>

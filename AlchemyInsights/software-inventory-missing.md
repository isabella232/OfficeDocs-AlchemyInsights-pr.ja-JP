---
title: ソフトウェアインベントリが存在しないか不正確です
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676613"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="11908-102">ソフトウェアインベントリが存在しないか不正確です</span><span class="sxs-lookup"><span data-stu-id="11908-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="11908-103">脅威と脆弱性の管理 (TVM) におけるソフトウェア インベントリとは、組織内の既知のソフトウェアを正式な共通プラットフォーム一覧 (CPE)　でリスト化したものです。</span><span class="sxs-lookup"><span data-stu-id="11908-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="11908-104">公式 CPEのないソフトウェア製品では、脆弱性が公開されません。</span><span class="sxs-lookup"><span data-stu-id="11908-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="11908-105">また、インベントリには、ベンダー名、弱点の数、脅威、露出しているデバイスの数などの詳細が記載されています。</span><span class="sxs-lookup"><span data-stu-id="11908-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="11908-106">デバイス上のソフトウェアの変更は、通常 2 時間以内にセキュリティ ポータルに反映されます。</span><span class="sxs-lookup"><span data-stu-id="11908-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="11908-107">ただし、時間がかかる場合もあります。</span><span class="sxs-lookup"><span data-stu-id="11908-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="11908-108">現在、強制的に同期させる方法はありません。これは継続的な評価です。</span><span class="sxs-lookup"><span data-stu-id="11908-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="11908-109">ソフトウェアの変更後、5 時間経過しても TVM に変更が正確に反映されない場合は、以下の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="11908-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="11908-110">ソフトウェアがどのように検出されたかについては、ソフトウェア エビデンス セクションを確認してください。</span><span class="sxs-lookup"><span data-stu-id="11908-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="11908-111">ソフトウェアがサポートされているかどうか確認してください。</span><span class="sxs-lookup"><span data-stu-id="11908-111">Make sure that the software is supported.</span></span> <span data-ttu-id="11908-112">ソフトウェアは、現在、脅威や脆弱性の管理に対応していなくても、デバイス レベルでしか表示することができない場合があります。</span><span class="sxs-lookup"><span data-stu-id="11908-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="11908-113">ただし、限られたデータのみ使用可能です。</span><span class="sxs-lookup"><span data-stu-id="11908-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="11908-114">ポータルで誤りを報告する手順については、「[誤りを報告する](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11908-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="11908-115">**注**: MDE ポータルでの誤りの報告は、エンジニアリングへの一方通行のチャネルです。</span><span class="sxs-lookup"><span data-stu-id="11908-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="11908-116">緊急性の高い問題の場合は、サポート チケットを開きます。</span><span class="sxs-lookup"><span data-stu-id="11908-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="11908-117">詳細については、「[ソフトウェアインベントリ - 脅威と脆弱性の管理](/microsoft-365/security/defender-endpoint/tvm-software-inventory)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11908-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>
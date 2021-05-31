---
title: Exchange Online PowerShell のマイクロ遅延またはスロットル
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
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702131"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="e7124-102">Exchange Online PowerShell のマイクロ遅延またはスロットル</span><span class="sxs-lookup"><span data-stu-id="e7124-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="e7124-103">Exchange Online でスクリプトとコマンドレットを実行すると、 "マイクロ遅延が適用されました" と警告または遅延が表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="e7124-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="e7124-104">これを解決する方法をいくつか提案します。</span><span class="sxs-lookup"><span data-stu-id="e7124-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="e7124-105">診断を実行して、テナントの PowerShell スロットル ポリシーを緩和してください。</span><span class="sxs-lookup"><span data-stu-id="e7124-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="e7124-106">このソリューションは、ほとんどの問題を解決します。</span><span class="sxs-lookup"><span data-stu-id="e7124-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="e7124-107">それでも問題が解決しない場合は、[Exchange Online v2 PowerShell モジュール](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)を使用してください。これには REST API に基づくコマンドレットが含まれており、格段に高性能です。</span><span class="sxs-lookup"><span data-stu-id="e7124-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="e7124-108">これは、頻繁に使用される多くの Get- CMDlets に最適なソリューションになることがあります。</span><span class="sxs-lookup"><span data-stu-id="e7124-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="e7124-109">v2 モジュールには含まれていないコマンドレットを使用する必要がある場合は、「[Office 365 で多数のユーザー向けに PowerShell コマンドレットを実行する](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)」を参照してください。これは、Exchange Online の PowerShell スロットル制限を回避する方法について説明しています。</span><span class="sxs-lookup"><span data-stu-id="e7124-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>

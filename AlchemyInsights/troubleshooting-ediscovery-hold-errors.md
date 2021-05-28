---
title: 電子情報開示で発生するエラーのトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676593"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="93d68-102">電子情報開示で発生するエラーのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="93d68-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="93d68-103">電子情報開示で問題が発生していますか?</span><span class="sxs-lookup"><span data-stu-id="93d68-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="93d68-104">こちらに、推奨されるベスト プラクティスの一部を示します。</span><span class="sxs-lookup"><span data-stu-id="93d68-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="93d68-105">保持している配布状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="93d68-105">Check the hold distribution status.</span></span>  <span data-ttu-id="93d68-106">状態が **オン (保留中)** または **オフ (保留中)** である場合は、配布の保持を待機して完了します。</span><span class="sxs-lookup"><span data-stu-id="93d68-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="93d68-107">電子情報開示の更新の保持を、トランザクションごとに繰り返しポリシーを更新するのではなく、1 つの一括要求に結合します。</span><span class="sxs-lookup"><span data-stu-id="93d68-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="93d68-108">Set-CaseHoldPolicy <policyname> の実行 - RetryDistribution を セキュリティ/コンプライアンス センター Powershell で実行します。</span><span class="sxs-lookup"><span data-stu-id="93d68-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="93d68-109">詳細については、「[セキュリティ/コンプライアンス センターの PowerShell に接続する](/powershell/exchange/connect-to-scc-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93d68-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="93d68-110">これらの設定を確認する手順や、電子情報開示の保持の問題を解決するためのその他のベスト プラクティスについては、「[電子情報開示の保持エラーのトラブルシューティング](/microsoft-365/compliance/hold-distribution-errors)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93d68-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="93d68-111">その他の一般的な電子情報開示の問題のトラブルシューティングについては、[電子情報開示に共通する問題の調査、トラブルシューティング、問題解決](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)」をご参照ください。</span><span class="sxs-lookup"><span data-stu-id="93d68-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>

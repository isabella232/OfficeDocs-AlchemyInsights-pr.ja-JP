---
title: コンテンツ検索の結果がありません
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516784"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="923c0-102">コンテンツ検索/エクスポートからの結果がありません</span><span class="sxs-lookup"><span data-stu-id="923c0-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="923c0-103">コンテンツ検索/エクスポートに関する問題は、特定の管理者によってセットアップされた特定のコンプライアンスセキュリティフィルターによって、すべての管理者に伝達されないため、データが返されないことがあります。</span><span class="sxs-lookup"><span data-stu-id="923c0-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="923c0-104">この問題を解決するには、以下の原因と考えられるコンプライアンスセキュリティフィルターがあるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="923c0-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="923c0-105">セキュリティとコンプライアンスセンターの Powershell への接続</span><span class="sxs-lookup"><span data-stu-id="923c0-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="923c0-106">次のコマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="923c0-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="923c0-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="923c0-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="923c0-108">New-compliancesecurityfilter-組織 $org</span><span class="sxs-lookup"><span data-stu-id="923c0-108">Get-ComplianceSecurityFilter -Organization $org</span></span>
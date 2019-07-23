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
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/19/2019
ms.locfileid: "35810582"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="fd7f9-102">コンテンツ検索/エクスポートからの結果がありません</span><span class="sxs-lookup"><span data-stu-id="fd7f9-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="fd7f9-103">コンテンツ検索/エクスポートに関する問題は、特定の管理者によってセットアップされた特定のコンプライアンスセキュリティフィルターによって、すべての管理者に伝達されないため、データが返されないことがあります。</span><span class="sxs-lookup"><span data-stu-id="fd7f9-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="fd7f9-104">この問題を解決するには、以下の原因と考えられるコンプライアンスセキュリティフィルターがあるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="fd7f9-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="fd7f9-105">セキュリティとコンプライアンスセンターの Powershell への接続</span><span class="sxs-lookup"><span data-stu-id="fd7f9-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="fd7f9-106">次のコマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="fd7f9-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="fd7f9-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="fd7f9-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="fd7f9-108">New-compliancesecurityfilter-組織 $org</span><span class="sxs-lookup"><span data-stu-id="fd7f9-108">Get-ComplianceSecurityFilter -Organization $org</span></span>
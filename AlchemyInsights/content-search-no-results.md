---
title: コンテンツ検索の結果がない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680652"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="9f022-102">コンテンツ検索 / エクスポートの結果がない</span><span class="sxs-lookup"><span data-stu-id="9f022-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="9f022-103">コンテンツ検索 / エクスポートでデータが何も返されない問題は、特定の管理者によりセットアップされたものの、すべての管理者には伝達されなかった特定のコンプライアンス セキュリティ フィルターが原因の可能性があります。</span><span class="sxs-lookup"><span data-stu-id="9f022-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="9f022-104">この問題を解決するには、原因となっている可能性があるコンプライアンス セキュリティ フィルターがないかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="9f022-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="9f022-105">セキュリティ/コンプライアンス センターの PowerShell に接続します。</span><span class="sxs-lookup"><span data-stu-id="9f022-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="9f022-106">次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="9f022-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="9f022-107">$org = “yourdomain.com”</span><span class="sxs-lookup"><span data-stu-id="9f022-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="9f022-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="9f022-108">Get-ComplianceSecurityFilter -Organization $org</span></span>
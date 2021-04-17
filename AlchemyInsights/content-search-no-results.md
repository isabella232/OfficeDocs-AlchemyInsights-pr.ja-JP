---
title: コンテンツ検索の結果がない
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816853"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="f7884-102">コンテンツ検索 / エクスポートの結果がない</span><span class="sxs-lookup"><span data-stu-id="f7884-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="f7884-103">コンテンツ検索 / エクスポートでデータが何も返されない問題は、特定の管理者によりセットアップされたものの、すべての管理者には伝達されなかった特定のコンプライアンス セキュリティ フィルターが原因の可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f7884-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="f7884-104">この問題を解決するには、原因となっている可能性があるコンプライアンス セキュリティ フィルターがないかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="f7884-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="f7884-105">セキュリティ/コンプライアンス センターの PowerShell に接続します。</span><span class="sxs-lookup"><span data-stu-id="f7884-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="f7884-106">次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="f7884-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="f7884-107">$org = “yourdomain.com”</span><span class="sxs-lookup"><span data-stu-id="f7884-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="f7884-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="f7884-108">Get-ComplianceSecurityFilter -Organization $org</span></span>
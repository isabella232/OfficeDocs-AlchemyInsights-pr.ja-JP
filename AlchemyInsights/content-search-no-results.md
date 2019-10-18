---
title: コンテンツ検索の結果がない
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516784"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="90391-102">コンテンツ検索 / エクスポートの結果がない</span><span class="sxs-lookup"><span data-stu-id="90391-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="90391-103">コンテンツ検索 / エクスポートでデータが何も返されない問題は、特定の管理者によりセットアップされたものの、すべての管理者には伝達されなかった特定のコンプライアンス セキュリティ フィルターが原因の可能性があります。</span><span class="sxs-lookup"><span data-stu-id="90391-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="90391-104">この問題を解決するには、原因となっている可能性があるコンプライアンス セキュリティ フィルターがないかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="90391-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="90391-105">セキュリティ/コンプライアンス センターの PowerShell に接続します。</span><span class="sxs-lookup"><span data-stu-id="90391-105">Connect to Security and Compliance Center PowerShell.</span></span>
2. <span data-ttu-id="90391-106">次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="90391-106">Run the following:</span></span>
<br><span data-ttu-id="90391-107">$org = “yourdomain.com”</span><span class="sxs-lookup"><span data-stu-id="90391-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="90391-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="90391-108">Get-ComplianceSecurityFilter -Organization $org</span></span>
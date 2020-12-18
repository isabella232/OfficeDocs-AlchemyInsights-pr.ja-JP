---
title: コンテンツ検索/エクスポート中に結果が返されない
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680577"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="e8429-102">コンテンツ検索/エクスポート中に結果が返されない</span><span class="sxs-lookup"><span data-stu-id="e8429-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="e8429-103">次の電子情報開示のシナリオで問題が発生している場合:</span><span class="sxs-lookup"><span data-stu-id="e8429-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="e8429-104">コンテンツ検索/エクスポートは、データを返さないか、期待外のデータを返します。</span><span class="sxs-lookup"><span data-stu-id="e8429-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="e8429-105">電子情報開示の検索またはエクスポートが失敗する</span><span class="sxs-lookup"><span data-stu-id="e8429-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="e8429-106">特定の管理者によってセットアップされ、すべての管理者に通知されなかった特定のコンプライアンス セキュリティ フィルターが原因で、この問題が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="e8429-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="e8429-107">この問題を解決するには、原因となっている可能性があるコンプライアンス セキュリティ フィルターがないかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="e8429-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="e8429-108">セキュリティ/コンプライアンス センターの PowerShell に接続します。</span><span class="sxs-lookup"><span data-stu-id="e8429-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="e8429-109">次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="e8429-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="e8429-110">コンプライアンス セキュリティ フィルターの詳細については、「[コンテンツ検索のアクセス許可フィルター](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8429-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>

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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727228"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="1eb4c-102">コンテンツ検索/エクスポート中に結果が返されない</span><span class="sxs-lookup"><span data-stu-id="1eb4c-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="1eb4c-103">次の電子情報開示のシナリオで問題が発生している場合:</span><span class="sxs-lookup"><span data-stu-id="1eb4c-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="1eb4c-104">コンテンツ検索/エクスポートは、データを返さないか、期待外のデータを返します。</span><span class="sxs-lookup"><span data-stu-id="1eb4c-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="1eb4c-105">電子情報開示の検索またはエクスポートが失敗する</span><span class="sxs-lookup"><span data-stu-id="1eb4c-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="1eb4c-106">これは、特定の管理者によってセットアップされ、すべての管理者に伝達されていない特定のコンプライアンス セキュリティ フィルターが原因である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1eb4c-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="1eb4c-107">この問題を解決するには、原因となっている可能性があるコンプライアンス セキュリティ フィルターがないかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="1eb4c-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="1eb4c-108">セキュリティ/コンプライアンス センターの PowerShell に接続します。</span><span class="sxs-lookup"><span data-stu-id="1eb4c-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="1eb4c-109">次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="1eb4c-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="1eb4c-110">コンプライアンス セキュリティ フィルターの詳細については、「[コンテンツ検索のアクセス許可フィルター](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1eb4c-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>

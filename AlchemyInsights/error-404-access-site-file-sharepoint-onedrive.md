---
title: 'エラー 404: ファイルが見つかりません'
ms.author: kirks
author: Techwriter40
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 1610ba60ad7c632cb3b2afab79d58aff4e171c93
ms.sourcegitcommit: 20b6a1fb3f0d899f3b204e3c066262d10623a4ea
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35902898"
---
# <a name="error-404-file-not-found"></a><span data-ttu-id="4e7a6-102">エラー 404: ファイルが見つかりません</span><span class="sxs-lookup"><span data-stu-id="4e7a6-102">Error 404: File not found</span></span>

<span data-ttu-id="4e7a6-103">**エラー 404:** ユーザーが SharePoint または OneDrive のサイトまたはファイルにアクセスしようとしたときに、ファイルが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="4e7a6-103">**Error 404: File not found** is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="4e7a6-104">これは、サイトまたはファイルまたはグループの名前を変更、移動、または削除することによって発生することがよくあります。</span><span class="sxs-lookup"><span data-stu-id="4e7a6-104">This is often caused by a site or file or group getting renamed, moved, or deleted.</span></span>
<span data-ttu-id="4e7a6-105">ユーザーは、ルートサイトコレクションにアクセスしようとすると、エラーが発生し、削除されています。</span><span class="sxs-lookup"><span data-stu-id="4e7a6-105">Users will experience the error when attempting to access the root site collection and it has been deleted.</span></span>

<span data-ttu-id="4e7a6-106">この問題を解決するには、次のようにしてください。</span><span class="sxs-lookup"><span data-stu-id="4e7a6-106">The following can help with resolving this issue:</span></span>
- <span data-ttu-id="4e7a6-107">新しい[SharePoint 管理センターで、削除されたサイト](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center)(通信、グループに接続されたサイト、またはその他のサイト) について、新しい管理センターのプレビューに表示および復元します。</span><span class="sxs-lookup"><span data-stu-id="4e7a6-107">[View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center):  For modern sites (communication, group-connected, or other sites) that exist in the new admin center preview.</span></span>
- <span data-ttu-id="4e7a6-108">[Sharepoint サイトのごみ箱内のアイテムを復元](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be)する: 名前が変更されているファイル (または他のアイテム) を解決するには、sharepoint または OneDrive サイトに移動し、サイトコンテンツからごみ箱を表示します。</span><span class="sxs-lookup"><span data-stu-id="4e7a6-108">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be):  To resolve file (or other item) that has been renamed, moved or deleted go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span>
- <span data-ttu-id="4e7a6-109">[Office 365 セキュリティ&amp;コンプライアンスセンターで監査ログを検索](https://support.office.com/client/search-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c)します。アイテムをまだ検索できない場合は、監査ログを検索します (ログが有効な場合)。</span><span class="sxs-lookup"><span data-stu-id="4e7a6-109">[Search the audit log in the Office 365 Security &amp; Compliance Center](https://support.office.com/client/search-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c):  Search the audit log (if logging is enabled) if you are still unable to find the item.</span></span>
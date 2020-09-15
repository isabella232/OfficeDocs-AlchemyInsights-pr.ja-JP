---
title: 'エラー 404: ファイルが見つかりません'
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d8e0d855e1e5fe702d468c0a4075a6f3264e67c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709228"
---
# <a name="error-404-file-not-found-in-sharepoint-or-onedrive"></a><span data-ttu-id="c9b17-102">エラー 404: ファイルが SharePoint または OneDrive に見つかりません</span><span class="sxs-lookup"><span data-stu-id="c9b17-102">Error 404: File not found in SharePoint or OneDrive</span></span>

<span data-ttu-id="c9b17-103">**エラー 404: ファイルが見つかりません**は、ユーザーが SharePoint または OneDrive のサイトやファイルにアクセスしようとしたときに表示されます。</span><span class="sxs-lookup"><span data-stu-id="c9b17-103">**Error 404: File not found** is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="c9b17-104">多くの場合、これはサイト、ファイル、またはグループの名前変更や移動、削除が原因です。</span><span class="sxs-lookup"><span data-stu-id="c9b17-104">This is often caused by a site or file or group getting renamed, moved, or deleted.</span></span>
<span data-ttu-id="c9b17-105">ユーザーがルート サイト コレクションにアクセスしようとしたときに、そのサイト コレクションが削除されているとこのエラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="c9b17-105">Users will experience the error when attempting to access the root site collection and it has been deleted.</span></span>

<span data-ttu-id="c9b17-106">この問題を解決するために、次の操作を行ってください。</span><span class="sxs-lookup"><span data-stu-id="c9b17-106">The following can help with resolving this issue:</span></span>
- <span data-ttu-id="c9b17-107">[新しい SharePoint 管理センターで削除されたサイトを表示および復元する](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center): 新しい管理センター (プレビュー版) に存在するモダン サイト (コミュニケーション サイトやグループ接続サイトなど) については、こちらを参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9b17-107">[View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center):  For modern sites (communication, group-connected, or other sites) that exist in the new admin center preview.</span></span>
- <span data-ttu-id="c9b17-108">[SharePoint サイトのごみ箱のアイテムを復元する](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be): ファイル (またはその他のアイテム) が名前変更、移動または削除されていた場合の問題を解決するには、SharePoint または OneDrive サイトに移動し、サイト コンテンツからごみ箱を表示します。</span><span class="sxs-lookup"><span data-stu-id="c9b17-108">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be):  To resolve file (or other item) that has been renamed, moved or deleted go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span>
- <span data-ttu-id="c9b17-109">[セキュリティ&amp;コンプライアンス センターで監査ログを検索する](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance): それでもアイテムが見つからない場合は、監査ログを検索してください (ログが有効になっている場合)。</span><span class="sxs-lookup"><span data-stu-id="c9b17-109">[Search the audit log in the Security &amp; Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance):  Search the audit log (if logging is enabled) if you are still unable to find the item.</span></span>
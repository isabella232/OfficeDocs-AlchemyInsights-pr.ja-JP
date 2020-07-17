---
title: エラー 404、ファイルが見つかりませんのトラブルシューティング、
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: c860b9db63e8d341cbe5e6d8d1d420b4c9d01c9f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505348"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="387f3-102">エラー 404、ファイルが見つかりませんのトラブルシューティング、</span><span class="sxs-lookup"><span data-stu-id="387f3-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="387f3-103">ユーザーが SharePoint または OneDrive のサイトまたはファイルにアクセスしようとしたときに、エラー 404 が表示されます。</span><span class="sxs-lookup"><span data-stu-id="387f3-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="387f3-104">これは多くの場合、サイト、ファイル、またはグループの名前変更、移動、または削除が原因です。</span><span class="sxs-lookup"><span data-stu-id="387f3-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="387f3-105">たとえば、ユーザーがルート サイト コレクションにアクセスしようとすると 404 エラーが発生し、削除されました。</span><span class="sxs-lookup"><span data-stu-id="387f3-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="387f3-106">名前を変更、移動、または削除されたサイトのエラー 404 を解決するには:</span><span class="sxs-lookup"><span data-stu-id="387f3-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="387f3-107">従来の管理センターにある従来のサイトについては、「[削除されたサイト コレクションを復元する](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="387f3-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="387f3-108">新しい SharePoint 管理センターにある最新のサイト (通信、グループ接続、またはその他のサイト) については、「[新しい SharePoint 管理センターで削除されたサイトを表示または復元する](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="387f3-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="387f3-109">名前の変更、移動、または削除されたファイル (またはその他の項目) のエラー 404 を解決するには:</span><span class="sxs-lookup"><span data-stu-id="387f3-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="387f3-110">SharePoint または OneDrive サイトに移動し、サイト コンテンツからごみ箱を表示します。</span><span class="sxs-lookup"><span data-stu-id="387f3-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="387f3-111">詳細については、「[SharePoint サイトのごみ箱のアイテムを復元する](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="387f3-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="387f3-112">それでもアイテムが見つからない場合は、ログ記録が有効になっていると監査ログを検索できます。「[Microsoft 365 のセキュリティ センターとコンプライアンス センターで監査ログを検索する](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="387f3-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>

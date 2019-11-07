---
title: 2609-保持または電子情報開示の保留
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/05/2019
ms.locfileid: "38006840"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="e7f8c-102">SharePoint Online または OneDrive for Business のアイテムを削除できません</span><span class="sxs-lookup"><span data-stu-id="e7f8c-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="e7f8c-103">ユーザーが sharepoint Online または OneDrive for business のアイテムを削除できない場合があります。これは、アイテム保持ポリシー、保持ラベル、または電子情報開示の保留が OneDrive サイトの SharePoint または特定のアイテムに適用されるためです。</span><span class="sxs-lookup"><span data-stu-id="e7f8c-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="e7f8c-104">これには、ドキュメント、ドキュメントバージョン、フォルダー、ドキュメントライブラリ、リスト、アプリ、サイト、サイトコレクションを削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="e7f8c-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="e7f8c-105">保持されているアイテムを削除しようとした場合に表示されるエラーメッセージの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7f8c-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="e7f8c-106">"このサイトは、電子情報開示の保留またはアイテム保持ポリシーに含まれているため、削除できません"</span><span class="sxs-lookup"><span data-stu-id="e7f8c-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="e7f8c-107">"このサイトには、削除をブロックするためのコンプライアンスポリシーが設定されています。</span><span class="sxs-lookup"><span data-stu-id="e7f8c-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="e7f8c-108">"コンプライアンスポリシーは現在、このサイトの削除をブロックしています"</span><span class="sxs-lookup"><span data-stu-id="e7f8c-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="e7f8c-109">"このサイトコレクションは、電子情報開示の保留またはアイテム保持ポリシーに含まれるサイトが含まれているため、削除できません。"</span><span class="sxs-lookup"><span data-stu-id="e7f8c-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="e7f8c-110">"フォルダーを削除する前に、このフォルダー内のすべてのアイテムを削除する必要があります"</span><span class="sxs-lookup"><span data-stu-id="e7f8c-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="e7f8c-111">"このアイテムのバージョンは、保留中またはアイテム保持ポリシーにあるため削除できません"</span><span class="sxs-lookup"><span data-stu-id="e7f8c-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="e7f8c-112">"保留中にアイテムを削除することはできません"</span><span class="sxs-lookup"><span data-stu-id="e7f8c-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="e7f8c-113">"このアイテムに適用されているラベルは、編集または削除されないようにします。</span><span class="sxs-lookup"><span data-stu-id="e7f8c-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="e7f8c-114">"保留中またはアイテム保持ポリシーでリストを削除できません"</span><span class="sxs-lookup"><span data-stu-id="e7f8c-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="e7f8c-115">"リストは、ブロックされている場合、またはアイテム保持ポリシーが適用されている場合は削除できません"</span><span class="sxs-lookup"><span data-stu-id="e7f8c-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="e7f8c-116">これらのいずれかのシナリオでアイテムを削除するには、アイテム保持ポリシー、保持ラベル、または電子情報開示ホールドを削除する必要があります (または、サイトをアイテム保持ポリシーから除外する必要があります)。</span><span class="sxs-lookup"><span data-stu-id="e7f8c-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="e7f8c-117">この問題の原因となっている各保留リストを無効にするか、または除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7f8c-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="e7f8c-118">アイテム保持ポリシーまたはホールドを削除した後は、変更が反映されるまでに最大24時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="e7f8c-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="e7f8c-119">SharePoint サイトと OneDrive アカウントに適用できるさまざまな保持および保持機能の詳細については、以下のいずれかのトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7f8c-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="e7f8c-120">アイテム保持ポリシーの概要</span><span class="sxs-lookup"><span data-stu-id="e7f8c-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="e7f8c-121">保持ラベルの概要</span><span class="sxs-lookup"><span data-stu-id="e7f8c-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="e7f8c-122">詳細な電子情報開示で保留リストを管理する</span><span class="sxs-lookup"><span data-stu-id="e7f8c-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="e7f8c-123">電子情報開示の保持</span><span class="sxs-lookup"><span data-stu-id="e7f8c-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="e7f8c-124">従来のサイトの閉鎖および削除ポリシー</span><span class="sxs-lookup"><span data-stu-id="e7f8c-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)

---
title: 2609 の保持または電子情報開示の保留
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/05/2019
ms.locfileid: "38006840"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="89adb-102">SharePoint Online または OneDrive for Business でアイテムを削除できない</span><span class="sxs-lookup"><span data-stu-id="89adb-102">Unable to delete items in SharePoint or OneDrive</span></span>

<span data-ttu-id="89adb-103">ユーザーが SharePoint Online または OneDrive for Business のアイテムを削除できない場合があります。これは、アイテム保持ポリシー、保持ラベル、または電子情報開示の保留が OneDrive サイトの SharePoint サイトや特定のアイテムに適用されているためです。</span><span class="sxs-lookup"><span data-stu-id="89adb-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="89adb-104">この場合、ドキュメント、ドキュメントのバージョン、フォルダー、ドキュメント ライブラリ、リスト、アプリ、サイト、またはサイト コレクションを削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="89adb-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="89adb-105">保持されているアイテムを削除しようとすると、次のエラーメッセージが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="89adb-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="89adb-106">"このサイトは、電子情報開示の保留またはアイテム保持ポリシーに含まれているため削除できません"</span><span class="sxs-lookup"><span data-stu-id="89adb-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="89adb-107">"このサイトには、削除をブロックするコンプライアンス ポリシーが設定されています"</span><span class="sxs-lookup"><span data-stu-id="89adb-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="89adb-108">"コンプライアンス ポリシーは現在このサイトの削除をブロックしています"</span><span class="sxs-lookup"><span data-stu-id="89adb-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="89adb-109">"このサイト コレクションは、電子情報開示の保留またはアイテム保持ポリシーに含まれているサイトを含むため削除できません"</span><span class="sxs-lookup"><span data-stu-id="89adb-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="89adb-110">"フォルダーを削除する前に、このフォルダー内のすべてのアイテムを削除する必要があります"</span><span class="sxs-lookup"><span data-stu-id="89adb-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="89adb-111">"このアイテムのバージョンは保留中であるか、またはアイテム保持ポリシーにより、削除できません。</span><span class="sxs-lookup"><span data-stu-id="89adb-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="89adb-112">"保留中のアイテムを削除することはできません"</span><span class="sxs-lookup"><span data-stu-id="89adb-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="89adb-113">このアイテムに適用されるラベルにより、編集や削除ができません。</span><span class="sxs-lookup"><span data-stu-id="89adb-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="89adb-114">"保留中またはアイテム保持ポリシーにより、リストを削除することはできません"</span><span class="sxs-lookup"><span data-stu-id="89adb-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="89adb-115">"リストがブロックされている場合やアイテム保持ポリシーが適用されている場合は削除できません"</span><span class="sxs-lookup"><span data-stu-id="89adb-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="89adb-116">これらのシナリオでアイテムを削除するには、アイテム保持ポリシー、保持ラベル、または電子情報開示の保留を削除する必要があります (または、サイトをアイテム保持ポリシーから除外する必要があります)。</span><span class="sxs-lookup"><span data-stu-id="89adb-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="89adb-117">この問題の原因となっている保留を無効にするか除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="89adb-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="89adb-118">アイテム保持ポリシーまたは保留を削除すると、この変更が反映されるまでに最大で 24 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="89adb-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="89adb-119">SharePoint サイトや OneDrive アカウントに適用できるさまざまな保持機能と保留機能については、次のいずれかのトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="89adb-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="89adb-120">アイテム保持ポリシーの概要</span><span class="sxs-lookup"><span data-stu-id="89adb-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="89adb-121">保持ラベルの概要</span><span class="sxs-lookup"><span data-stu-id="89adb-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="89adb-122">Advanced eDiscovery の保留を管理する</span><span class="sxs-lookup"><span data-stu-id="89adb-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="89adb-123">電子情報開示の保留</span><span class="sxs-lookup"><span data-stu-id="89adb-123">eDiscovery and holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="89adb-124">従来のサイト クローズと削除のポリシー</span><span class="sxs-lookup"><span data-stu-id="89adb-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)

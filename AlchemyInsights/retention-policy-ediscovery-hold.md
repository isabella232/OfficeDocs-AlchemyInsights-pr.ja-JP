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
ms.openlocfilehash: 3e60f0fc53cd78c9cc816a658a9df05e9075e26e
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571327"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="25777-102">SharePoint Online または OneDrive for Business でアイテムを削除できない</span><span class="sxs-lookup"><span data-stu-id="25777-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="25777-103">ユーザーが SharePoint Online または OneDrive for Business のアイテムを削除できない場合があります。これは、アイテム保持ポリシー、保持ラベル、または電子情報開示の保留が OneDrive サイトの SharePoint サイトや特定のアイテムに適用されているためです。</span><span class="sxs-lookup"><span data-stu-id="25777-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="25777-104">この場合、ドキュメント、ドキュメントのバージョン、フォルダー、ドキュメント ライブラリ、リスト、アプリ、サイト、またはサイト コレクションを削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="25777-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> 

<span data-ttu-id="25777-105">これらのシナリオでアイテムを削除するには、アイテム保持ポリシー、保持ラベル、または電子情報開示の保留を削除する必要があります (または、サイトをアイテム保持ポリシーから除外する必要があります)。</span><span class="sxs-lookup"><span data-stu-id="25777-105">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="25777-106">この問題の原因となっている保留を無効にするか除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="25777-106">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="25777-107">アイテム保持ポリシーまたは保留を削除すると、この変更が反映されるまでに最大で 24 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="25777-107">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="25777-108">SharePoint サイトや OneDrive アカウントに適用できるさまざまな保持機能と保留機能については、次のいずれかのトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="25777-108">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="25777-109">アイテム保持ポリシーの概要</span><span class="sxs-lookup"><span data-stu-id="25777-109">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)
- [<span data-ttu-id="25777-110">保持ラベルの概要</span><span class="sxs-lookup"><span data-stu-id="25777-110">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)
- [<span data-ttu-id="25777-111">Advanced eDiscovery の保留を管理する</span><span class="sxs-lookup"><span data-stu-id="25777-111">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)
- [<span data-ttu-id="25777-112">電子情報開示の保留</span><span class="sxs-lookup"><span data-stu-id="25777-112">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)
- [<span data-ttu-id="25777-113">従来のサイト クローズと削除のポリシー</span><span class="sxs-lookup"><span data-stu-id="25777-113">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
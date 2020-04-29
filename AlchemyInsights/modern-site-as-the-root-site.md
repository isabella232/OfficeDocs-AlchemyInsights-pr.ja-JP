---
title: ルートサイトとしてのモダン サイト
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713796"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="89591-102">ルート サイトとしてのモダン サイト</span><span class="sxs-lookup"><span data-stu-id="89591-102">Modern site as root site</span></span>

<span data-ttu-id="89591-103">[モダン サイトと従来のサイトのルートサイトを交換](https://docs.microsoft.com/sharepoint/modern-root-site)できるようにするために、新機能のロールアウトを開始しました。</span><span class="sxs-lookup"><span data-stu-id="89591-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="89591-104">[Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) を使用して、元のサイトをアーカイブしながら、別のサイトとサイトの場所を交換します。</span><span class="sxs-lookup"><span data-stu-id="89591-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="89591-105">チーム サイト (グループに接続されていない) とコミュニケーション サイトの両方で使用することができます。</span><span class="sxs-lookup"><span data-stu-id="89591-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="89591-106">モダン コミュニケーション サイトを作成するために、従来のルート サイトを削除しないでください。</span><span class="sxs-lookup"><span data-stu-id="89591-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="89591-107">このようなことは、Microsoft ではサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="89591-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="89591-108">ルートサイトを削除すると、サイトを復元するか、同じ URL の新しいサイトが作成されるまで、組織内のすべての SharePoint サイトですべてのユーザーにアクセスできなくなります。</span><span class="sxs-lookup"><span data-stu-id="89591-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="89591-109">私たちは、メッセージ センター経由でこの機能を伝えていきます。</span><span class="sxs-lookup"><span data-stu-id="89591-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="89591-110">すぐに、ユーザーのテナントの機能が有効になります。</span><span class="sxs-lookup"><span data-stu-id="89591-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="89591-111">サイトの入れ替えに関する既知の問題</span><span class="sxs-lookup"><span data-stu-id="89591-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="89591-112">ターゲット サイトでは、短時間の間、"見つかりません" (HTTP 404) というエラーを返す場合があります。</span><span class="sxs-lookup"><span data-stu-id="89591-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="89591-113">検索インデックスを更新するには、コンテンツが再クロールされる必要があります。</span><span class="sxs-lookup"><span data-stu-id="89591-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="89591-114">ここでは、要求される手動ステップはありません。これは自動的に行われます。</span><span class="sxs-lookup"><span data-stu-id="89591-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="89591-115">"静的" リンクに依存するもの (ファイルの同期や OneNote ファイルなど) は、手動で修正される必要があります。</span><span class="sxs-lookup"><span data-stu-id="89591-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="89591-116">Project Server サイトを検証し、それらが正しく関連付けられていることを確認することが必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="89591-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 

---
title: ルートサイトとしてのモダンサイト
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543858"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="4653a-102">ルートサイトとしてのモダンサイト</span><span class="sxs-lookup"><span data-stu-id="4653a-102">Modern site as root site</span></span>

<span data-ttu-id="4653a-103">従来のサイトのルートサイトをモダンサイトと入れ替えることができる新機能のロールアウトを開始しました。</span><span class="sxs-lookup"><span data-stu-id="4653a-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="4653a-104">元のサイトをアーカイブしている間は、 [Invoke-spsite wap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)を使用してサイトの場所を別のサイトと交換します。</span><span class="sxs-lookup"><span data-stu-id="4653a-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="4653a-105">両方のチームサイト (グループに接続されていない) とコミュニケーションサイトで使用できます。</span><span class="sxs-lookup"><span data-stu-id="4653a-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="4653a-106">モダンコミュニケーションサイトを作成するために、従来のルートサイトを削除しないでください。</span><span class="sxs-lookup"><span data-stu-id="4653a-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="4653a-107">これは Microsoft ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4653a-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="4653a-108">ルートサイトを削除すると、サイトを復元するか、同じ URL で新しいサイトを作成するまで、組織内のすべての SharePoint サイトがすべてのユーザーに対してアクセスできなくなります。</span><span class="sxs-lookup"><span data-stu-id="4653a-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="4653a-109">この機能は、メッセージセンター経由で通信します。</span><span class="sxs-lookup"><span data-stu-id="4653a-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="4653a-110">この機能は、すぐにテナントでオンになるはずです。</span><span class="sxs-lookup"><span data-stu-id="4653a-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="4653a-111">サイトのスワップに関する既知の問題</span><span class="sxs-lookup"><span data-stu-id="4653a-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="4653a-112">ターゲットサイトは、短時間に "not found" (HTTP 404) エラーを返す場合があります。</span><span class="sxs-lookup"><span data-stu-id="4653a-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="4653a-113">検索インデックスを更新するには、コンテンツを再クロールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="4653a-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="4653a-114">ここでは手動での手順は必要ありませんが、これは自動的に実行されます。</span><span class="sxs-lookup"><span data-stu-id="4653a-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="4653a-115">"静的" リンク (ファイル同期や OneNote ファイルなど) に依存するものは、手動で修正する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4653a-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="4653a-116">Project Server サイトが正しく関連付けられていることを確認するには、そのサイトを検証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4653a-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 

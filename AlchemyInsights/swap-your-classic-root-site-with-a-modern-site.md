---
title: モダン サイトとクラシック ルート サイトを入れ替える
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/07/2019
ms.locfileid: "36249510"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="b81a5-102">モダン サイトとクラシック ルート サイトを入れ替える</span><span class="sxs-lookup"><span data-stu-id="b81a5-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="b81a5-103">2019 年 4 月より前に環境を設定した場合は、Microsoft PowerShell を使用して、ルート サイトをモダン サイトに変更できます。</span><span class="sxs-lookup"><span data-stu-id="b81a5-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="b81a5-104">ルート サイトとして使用したい別のサイトをお持ちの場合は、そのサイトとルート サイトを置き換える (入れ替える) ことができます。</span><span class="sxs-lookup"><span data-stu-id="b81a5-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="b81a5-105">[Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) を使用して、元のサイトをアーカイブしながら、別のサイトとサイトの場所を交換します。</span><span class="sxs-lookup"><span data-stu-id="b81a5-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="b81a5-106">チーム サイト (グループに接続されていない) とコミュニケーション サイトの両方で使用できます。</span><span class="sxs-lookup"><span data-stu-id="b81a5-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="b81a5-107">間もなく、追加機能が導入されて、引き続きサイトのコンテンツを使用できるようになりますが、既存のサイトをコミュニケーション サイトに変換します。</span><span class="sxs-lookup"><span data-stu-id="b81a5-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="b81a5-108">これらの機能は、段階的にロールアウトされます。</span><span class="sxs-lookup"><span data-stu-id="b81a5-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="b81a5-109">更新プログラムに関しては、引き続き Office 365 メッセージ センターでご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b81a5-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="b81a5-110">サイトの入れ替えに関する既知の問題</span><span class="sxs-lookup"><span data-stu-id="b81a5-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="b81a5-111">ターゲット サイトでは、短時間の間、"見つかりません" (HTTP 404) というエラーを返す場合があります。</span><span class="sxs-lookup"><span data-stu-id="b81a5-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="b81a5-112">検索インデックスを更新するには、コンテンツが再クロールされる必要があります。</span><span class="sxs-lookup"><span data-stu-id="b81a5-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="b81a5-113">要求される手動ステップはありません。つまり、これは自動的に行われます。</span><span class="sxs-lookup"><span data-stu-id="b81a5-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="b81a5-114">"静的" リンクに依存するもの (ファイルの同期や OneNote ファイルなど) は、手動で修正される必要があります。</span><span class="sxs-lookup"><span data-stu-id="b81a5-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="b81a5-115">ソース サイトが組織のニュース サイトだった場合は、URL を更新します。</span><span class="sxs-lookup"><span data-stu-id="b81a5-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="b81a5-116"> すべての組織のニュース サイトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b81a5-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="b81a5-117">Project Server サイトを検証し、それらが正しく関連付けられていることを確認することが必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="b81a5-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>






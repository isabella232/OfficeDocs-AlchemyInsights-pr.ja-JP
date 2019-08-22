---
title: 従来のルートサイトをモダンサイトと入れ替える
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
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501084"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="a544f-102">従来のルートサイトをモダンサイトと入れ替える</span><span class="sxs-lookup"><span data-stu-id="a544f-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="a544f-103">4月2019日より前に環境を設定した場合は、Microsoft PowerShell を使用してルートサイトをモダンサイトに変更することができます。</span><span class="sxs-lookup"><span data-stu-id="a544f-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="a544f-104">ルートサイトとして使用する別のサイトがある場合は、ルートサイトを置き換える (スワップする) ことができます。</span><span class="sxs-lookup"><span data-stu-id="a544f-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="a544f-105">元のサイトをアーカイブしているときに、 [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)を使用してサイトの場所を別のサイトと交換します。</span><span class="sxs-lookup"><span data-stu-id="a544f-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="a544f-106">両方のチームサイト (グループに接続されていない) とコミュニケーションサイトで使用できます。</span><span class="sxs-lookup"><span data-stu-id="a544f-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="a544f-107">サイトのコンテンツを引き続き使用し、既存のサイトをコミュニケーションサイトに変換できる追加機能が導入されます。</span><span class="sxs-lookup"><span data-stu-id="a544f-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="a544f-108">これらの機能は段階的にロールアウトされます。</span><span class="sxs-lookup"><span data-stu-id="a544f-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="a544f-109">引き続き Office 365 メッセージセンターで更新プログラムをチェックします。</span><span class="sxs-lookup"><span data-stu-id="a544f-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="a544f-110">サイトのスワップに関する既知の問題</span><span class="sxs-lookup"><span data-stu-id="a544f-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="a544f-111">ターゲットサイトは、短時間に "not found" (HTTP 404) エラーを返す場合があります。</span><span class="sxs-lookup"><span data-stu-id="a544f-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="a544f-112">検索インデックスを更新するには、コンテンツを再クロールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a544f-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="a544f-113">手動による手順は必要ありません。これは自動的に実行されます。</span><span class="sxs-lookup"><span data-stu-id="a544f-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="a544f-114">"静的" リンク (ファイル同期や OneNote ファイルなど) に依存するものは、手動で修正する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a544f-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="a544f-115">ソースサイトが組織のニュースサイトの場合は、URL を更新します。</span><span class="sxs-lookup"><span data-stu-id="a544f-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="a544f-116">すべての組織のニュースサイトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="a544f-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="a544f-117">Project Server サイトが正しく関連付けられていることを確認するには、そのサイトを検証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a544f-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>






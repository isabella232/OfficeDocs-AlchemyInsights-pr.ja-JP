---
title: サイト探索を行う
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2021
ms.locfileid: "50696411"
---
# <a name="do-site-discovery"></a><span data-ttu-id="3bc24-102">サイト探索を行う</span><span class="sxs-lookup"><span data-stu-id="3bc24-102">Do site discovery</span></span>

<span data-ttu-id="3bc24-103">レガシ Web アプリケーションをまだ使用しており、Internet Explorer モードの使用を計画している場合 (ほとんどのお客様が該当)、追加のサイト探索の実行が必要になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3bc24-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="3bc24-104">**Microsoft Edge の以前のバージョンが既に展開されています**</span><span class="sxs-lookup"><span data-stu-id="3bc24-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="3bc24-105">Microsoft Edge のレガシ バージョンで使用するように、エンタープライズ サイト一覧が既に構成されている場合、サイト探索はほぼ完了しています。</span><span class="sxs-lookup"><span data-stu-id="3bc24-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="3bc24-106">ニュートラル サイトの追加が必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="3bc24-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="3bc24-107">ニュートラルサイトは、通常、シングル サインオン (SSO) を提供するサイトです。</span><span class="sxs-lookup"><span data-stu-id="3bc24-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="3bc24-108">Microsoft Edge からニュートラル サイトに移動する場合は、Microsoft Edge で認証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3bc24-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="3bc24-109">Internet Explorer モードでニュートラル サイトに移動する場合は、Internet Explorer モードで認証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3bc24-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="3bc24-110">使用する SSO またはその他のニュートラル サイトを特定し、エンタープライズ サイト一覧に追加します。</span><span class="sxs-lookup"><span data-stu-id="3bc24-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="3bc24-111">**既定のブラウザーが Internet Explorer の場合**</span><span class="sxs-lookup"><span data-stu-id="3bc24-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="3bc24-112">現在、Internet Explorer のみを使用している場合は、どのサイトが最新の Web 標準にアップグレードされ、どのサイトでまだ Internet Explorer が必要であるかを把握していない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3bc24-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="3bc24-113">これらのサイトを検索して、エンタープライズ サイト一覧に追加する必要があります。 これにより、必要なサイトでのみ Internet Explorer モードを使用できます。</span><span class="sxs-lookup"><span data-stu-id="3bc24-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="3bc24-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) を使用して、Internet Explorer モードを必要とする可能性があるサイトを検出します。</span><span class="sxs-lookup"><span data-stu-id="3bc24-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="3bc24-115">Windows 10、Windows 8.1、Windows 7 で、Windows Internet Explorer 8 から Internet Explorer 11 までを実行しているコンピューターでデータを収集できます。</span><span class="sxs-lookup"><span data-stu-id="3bc24-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="3bc24-116">**データを分析する**</span><span class="sxs-lookup"><span data-stu-id="3bc24-116">**Analyze the data**</span></span>

<span data-ttu-id="3bc24-117">サイト データを収集した後、次の 4 つの手順を実行してデータを分析することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="3bc24-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="3bc24-118">データをドメインごと、次に URL ごとに並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="3bc24-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="3bc24-119">Internet Explorer モード用に構成するアプリの境界を定義します。</span><span class="sxs-lookup"><span data-stu-id="3bc24-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="3bc24-120">アプリを定義するすべてのサイトと Web コントロールを含める必要があります。ただし、余分なサイトやコントロールを含めないようにします。</span><span class="sxs-lookup"><span data-stu-id="3bc24-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="3bc24-121">サイトによって、*https://contoso.com/app1* ように単純なものもあれば、複数のサイトやページを定義する必要があるものもあります。</span><span class="sxs-lookup"><span data-stu-id="3bc24-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="3bc24-122">アプリをテストして、ネイティブに機能していないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="3bc24-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="3bc24-123">多くのサイトでは、最新のブラウザーが検出されると最新のコンテンツが提供され、Internet Explorer が検出された場合にのみレガシ コンテンツが提供されます。</span><span class="sxs-lookup"><span data-stu-id="3bc24-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="3bc24-124">アプリがテストで失敗した場合は、エンタープライズ サイト一覧にアプリを追加します。</span><span class="sxs-lookup"><span data-stu-id="3bc24-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="3bc24-125">ベスト プラクティスとして、アプリを構成するすべてのサイトをグループ化することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="3bc24-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="3bc24-126">これにより、アプリをアップグレードするときに、サイト全体を Internet Explorer モードから削除し、そのアプリに最新のブラウザーを使用し始めるのが簡単になります。</span><span class="sxs-lookup"><span data-stu-id="3bc24-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="3bc24-127">サイト探索とデータの分析が完了すると、チャネル戦略の検索を開始する準備ができています。</span><span class="sxs-lookup"><span data-stu-id="3bc24-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>


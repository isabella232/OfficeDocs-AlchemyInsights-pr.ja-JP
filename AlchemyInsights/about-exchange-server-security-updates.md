---
title: Exchange Server のセキュリティ更新プログラムについて
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50484072"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="2e68f-102">Exchange Server のセキュリティ更新プログラムについて</span><span class="sxs-lookup"><span data-stu-id="2e68f-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="2e68f-103">マイクロソフトは、オンプレミスの Exchange Server 用の一連の重要なセキュリティ更新プログラムをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="2e68f-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="2e68f-104">影響を受けるサーバーのバージョンは、Exchange Server 2010、2013、2016、および 2019 の更新レベルです。</span><span class="sxs-lookup"><span data-stu-id="2e68f-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="2e68f-105">Exchange Online は影響を受けませんが、ハイブリッド構成のためにオンプレミスの Exchange サーバーがある場合、それらは潜在的に脆弱です。</span><span class="sxs-lookup"><span data-stu-id="2e68f-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="2e68f-106">オンプレミス サーバーを更新するには、少なくとも次のバージョンの Exchange を実行している必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e68f-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="2e68f-107">Exchange 2010 Service Pack 3</span><span class="sxs-lookup"><span data-stu-id="2e68f-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="2e68f-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="2e68f-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="2e68f-109">Exchange Server 2016 CU 19 または CU 18</span><span class="sxs-lookup"><span data-stu-id="2e68f-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="2e68f-110">Exchange Server 2019 CU 8 または CU 7</span><span class="sxs-lookup"><span data-stu-id="2e68f-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="2e68f-111">修正の場所については、次の発表を参照してください。[リリース: 2021 年 3 月 Exchange Server セキュリティ アップデート](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="2e68f-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="2e68f-112">**重要な注意点:**</span><span class="sxs-lookup"><span data-stu-id="2e68f-112">**Important notes:**</span></span>

<span data-ttu-id="2e68f-113">上記のリストのように、オンプレミス サーバーで必要な Exchange バージョンが実行されていない場合、更新プログラムのインストールは機能しません。</span><span class="sxs-lookup"><span data-stu-id="2e68f-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="2e68f-114">アップデートを手動でインストールする場合、重要な情報については、アップデート KB の記事の「既知の問題」セクションをお読みください。</span><span class="sxs-lookup"><span data-stu-id="2e68f-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="2e68f-115">セキュリティ更新プログラムは、昇格した CMD/PowerShell プロンプトから実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e68f-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>

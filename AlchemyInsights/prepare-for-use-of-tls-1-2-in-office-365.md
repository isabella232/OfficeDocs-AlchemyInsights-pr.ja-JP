---
title: Microsoft 365 で TLS 1.2 を使用するための準備
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085909"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="4ea16-102">Microsoft 365 で TLS 1.2 を使用するための準備</span><span class="sxs-lookup"><span data-stu-id="4ea16-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="4ea16-103">2018 年 10 月 31 日の時点で、Microsoft 365 では TLS 1.2 への移行が継続されます。</span><span class="sxs-lookup"><span data-stu-id="4ea16-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="4ea16-104">2020 年 10 月 15 日以降、O365 のサービス全体で TLS1.0 および 1.1 が非推奨になります。</span><span class="sxs-lookup"><span data-stu-id="4ea16-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="4ea16-105">この変更の展開は今後数週間から数か月にわたって継続されますが、2020 年 10 月 15 日以降、O365 を使用する場合、TLS 1.0 /1.1 の通話が機能しなくなることを想定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4ea16-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="4ea16-106">以前に連絡 (2017 年 12 月の MC126199、2018 年 2 月の MC128929、2019 年 7 月の MC186827、2020 年 7 月の MC218794) したように、クラス最高の暗号化を提供し、既定でサービスの安全性を高めるために、すべてのオンラインサービスをトランスポート層セキュリティ (TLS) 1.2 以上に移行しています。</span><span class="sxs-lookup"><span data-stu-id="4ea16-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="4ea16-107">お客様は、サーバーとリソースに TLS 1.0 / 1.1 を使用することも選択できますが、O365 リソースとやり取りする場合は TLS1.2 以降のみが機能します。</span><span class="sxs-lookup"><span data-stu-id="4ea16-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="4ea16-108">これらの変更の詳細については、[こちら](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)と[こちら](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4ea16-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  
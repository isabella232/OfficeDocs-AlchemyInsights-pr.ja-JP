---
title: SharePoint の移行中の調整
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "9000353"
- "1987"
- "9000136"
- "2968"
ms.assetid: ''
ms.openlocfilehash: dc77c462fcf32817c92709852e2d03ab2086b9a4
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958903"
---
# <a name="sharepoint-throttling"></a><span data-ttu-id="910db-102">SharePoint の調整</span><span class="sxs-lookup"><span data-stu-id="910db-102">SharePoint throttling</span></span>

<span data-ttu-id="910db-103">**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="910db-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="910db-104">**SharePoint Online の調整**</span><span class="sxs-lookup"><span data-stu-id="910db-104">**SharePoint Online throttling**</span></span>

<span data-ttu-id="910db-p101">SharePoint Online は、SharePoint Online サービスの最適なパフォーマンスと信頼性を維持する目的で調整を使用します。調整では、リソースの過剰な使用を防ぐため、ユーザー アクションまたは (スクリプトまたはコードによる) 同時呼び出しの数が制限されます。</span><span class="sxs-lookup"><span data-stu-id="910db-p101">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service. Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span>

<span data-ttu-id="910db-107">詳細については、次のリンクを参照してください。</span><span class="sxs-lookup"><span data-stu-id="910db-107">For more information please visit the links below:</span></span>

- [<span data-ttu-id="910db-108">SharePoint Online で調整またはブロックを回避する</span><span class="sxs-lookup"><span data-stu-id="910db-108">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)
- [<span data-ttu-id="910db-109">データ移行と SPO の調整</span><span class="sxs-lookup"><span data-stu-id="910db-109">Data Migration and SPO Throttling</span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)
- [<span data-ttu-id="910db-110">SharePoint Online と OneDrive の移行速度</span><span class="sxs-lookup"><span data-stu-id="910db-110">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
- [<span data-ttu-id="910db-111">指数関数的バックオフを使用して SharePoint Online の調整を処理する</span><span class="sxs-lookup"><span data-stu-id="910db-111">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)
- [<span data-ttu-id="910db-112">SharePoint Online のキャパシティ プランニングとロード テスト</span><span class="sxs-lookup"><span data-stu-id="910db-112">Capacity planning and load testing SharePoint Online</span></span>](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0)
- [<span data-ttu-id="910db-113">移行中にパフォーマンスが低下したり、スロットルが発生したりします</span><span class="sxs-lookup"><span data-stu-id="910db-113">I am experiencing poor performance or throttling during migration</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed#faq-and-troubleshooting)
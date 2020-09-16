---
title: パフォーマンスの問題 - SharePoint または OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771906"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="34aab-102">SharePoint または OneDrive において、処理が遅い、アクセスできない、または複数のユーザーで使用できない</span><span class="sxs-lookup"><span data-stu-id="34aab-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="34aab-103">SharePoint または OneDrive では、次のような理由で、処理が遅くなるか、アクセスできないか、またはサービスが利用できない、または503のエラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="34aab-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="34aab-104">SharePoint または OneDrive サイトの処理が遅かったり複数のユーザーに対して遅延が生じたりする場合、一時的なサービスの問題が発生している可能性があります。そのような状況では、ユーザーが SharePoint サイトまたは OneDrive コンテンツにアクセスする際に、一時的な遅延やナビゲーション エラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="34aab-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="34aab-105">[サービスの正常性ダッシュボード](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)を確認して、組織が影響を受けるかどうかを調べます。</span><span class="sxs-lookup"><span data-stu-id="34aab-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="34aab-106">ユーザーが SharePoint または OneDrive サイトに移動しようとしたときに、 *503 サーバーがビジー状態* であるというエラーが発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="34aab-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="34aab-107">このエラーは、SharePoint サービス内での調整が原因の可能性があります。</span><span class="sxs-lookup"><span data-stu-id="34aab-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="34aab-108">SharePoint Online は、SharePoint Online サービスの最適なパフォーマンスと信頼性を維持する目的で調整を使用します。</span><span class="sxs-lookup"><span data-stu-id="34aab-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="34aab-109">調整では、リソースの過剰な使用を防ぐため、ユーザー アクションまたは (スクリプトまたはコードによる) 同時呼び出しの数が制限されます。</span><span class="sxs-lookup"><span data-stu-id="34aab-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="34aab-110">調整の詳細については、「[SharePoint Online で調整またはブロックを回避する](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34aab-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="34aab-111">**クラシック**または**モダン**の SharePoint サイトまたはページでパフォーマンスの低下が発生した場合は、[ページ診断ツール](https://aka.ms/perftool)を利用してページの分析を行ってください。</span><span class="sxs-lookup"><span data-stu-id="34aab-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="34aab-112">全般的なパフォーマンス低下が引き続き発生する場合は、「[SharePoint Online のパフォーマンス チューニングの概要](https://go.microsoft.com/fwlink/?linkid=2024334)」の記事の下にあるリソースを参照してください。</span><span class="sxs-lookup"><span data-stu-id="34aab-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  
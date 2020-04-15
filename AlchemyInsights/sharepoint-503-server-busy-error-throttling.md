---
title: SharePoint Online の調整
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958739"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="852df-102">SharePoint Online の調整</span><span class="sxs-lookup"><span data-stu-id="852df-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="852df-103">**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="852df-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="852df-104">**「503 サーバーがビジー状態です」のエラー**</span><span class="sxs-lookup"><span data-stu-id="852df-104">**503 server is busy error**</span></span>

<span data-ttu-id="852df-105">ユーザーが SharePoint または OneDrive のサイトに移動しようとしたときに、"503 サーバーがビジー状態です" のエラーが発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="852df-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="852df-106">このエラーは、SharePoint サービス内での調整が原因の可能性があります。</span><span class="sxs-lookup"><span data-stu-id="852df-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="852df-107">SharePoint Online は、SharePoint Online サービスの最適なパフォーマンスと信頼性を維持する目的で調整を使用します。</span><span class="sxs-lookup"><span data-stu-id="852df-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="852df-108">調整では、リソースの過剰な使用を防ぐため、ユーザー アクションまたは (スクリプトまたはコードによる) 同時呼び出しの数が制限されます。</span><span class="sxs-lookup"><span data-stu-id="852df-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="852df-109">調整の詳細については、「[SharePoint Online で調整またはブロックを回避する](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="852df-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="852df-110">このエラーが調整に関連していないと考えられる場合は、[メッセージ センター](https://portal.office.com/adminportal/home#/MessageCenter)に移動して、テナントでアクティブ メンテナンスが実施されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="852df-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="852df-111">最後に、[サービス正常性](https://portal.office.com/adminportal/home#/servicehealth)ページにアクセスして、発生している可能性のあるインシデント/アドバイザリを確認してください。</span><span class="sxs-lookup"><span data-stu-id="852df-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>


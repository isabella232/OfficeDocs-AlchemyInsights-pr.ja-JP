---
title: SharePoint Online の調整
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751893"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="d0fb1-102">SharePoint Online の調整</span><span class="sxs-lookup"><span data-stu-id="d0fb1-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="d0fb1-103">ユーザーが SharePoint または OneDrive のサイトに移動しようとしたときに、"503 サーバーがビジー状態です" のエラーが発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="d0fb1-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="d0fb1-104">このエラーは、SharePoint サービス内での調整が原因の可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d0fb1-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="d0fb1-105">SharePoint Online は、SharePoint Online サービスの最適なパフォーマンスと信頼性を維持する目的で調整を使用します。</span><span class="sxs-lookup"><span data-stu-id="d0fb1-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="d0fb1-106">調整では、リソースの過剰な使用を防ぐため、ユーザー アクションまたは (スクリプトまたはコードによる) 同時呼び出しの数が制限されます。</span><span class="sxs-lookup"><span data-stu-id="d0fb1-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="d0fb1-107">調整の対象になる場合、99% の確率でカスタム コードが原因であるといえます。</span><span class="sxs-lookup"><span data-stu-id="d0fb1-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="d0fb1-108">調整の詳細については、「[SharePoint Online で調整またはブロックを回避する](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0fb1-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span></span>

<span data-ttu-id="d0fb1-109">このエラーが調整に関連していないと考えられる場合は、[メッセージ センター](https://portal.office.com/adminportal/home#/MessageCenter)に移動して、テナントでアクティブ メンテナンスが実施されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="d0fb1-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="d0fb1-110">最後に、[サービス正常性](https://portal.office.com/adminportal/home#/servicehealth)ページにアクセスして、発生している可能性のあるインシデント/アドバイザリを確認してください。</span><span class="sxs-lookup"><span data-stu-id="d0fb1-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>


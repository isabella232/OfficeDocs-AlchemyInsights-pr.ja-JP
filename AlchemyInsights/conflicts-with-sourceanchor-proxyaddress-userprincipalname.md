---
title: SourceAnchor、ProxyAddress、UserPrincipalNameとの競合
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198671"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="693b7-102">SourceAnchor、ProxyAddress、UserPrincipalNameとの競合</span><span class="sxs-lookup"><span data-stu-id="693b7-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="693b7-103">同期中に「同じ ProxyAddress または UserPrincipalName を持つ同期オブジェクトがディレクトリに存在する」などのエラーを受け取った場合は、「[重複した属性の同期エラーの診断と修正](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="693b7-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="693b7-104">また、重複属性の回復力を有効にすることを検討してください。</span><span class="sxs-lookup"><span data-stu-id="693b7-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="693b7-105">詳細については、「[IDの同期と重複属性の回復性](https://aka.ms/duplicateattributeresiliency)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="693b7-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>
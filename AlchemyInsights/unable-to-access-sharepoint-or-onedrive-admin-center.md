---
title: SharePoint または OneDrive 管理センターにアクセスできません
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 627a4ef2900a6b9bbef7eb3f3a214ee7c371e354
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716460"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="513d3-102">SharePoint または OneDrive 管理センターにアクセスできません</span><span class="sxs-lookup"><span data-stu-id="513d3-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="513d3-103">SharePoint または OneDrive 管理センターがアクセス不可、あるいは利用できない場合、一時的なサービスの問題が発生している可能性があります。そのような状況では、ユーザーが SharePoint サイトまたは OneDrive コンテンツにアクセスする際に、一時的な遅延やナビゲーション エラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="513d3-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="513d3-104">[サービスの正常性ダッシュボード](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)を確認して、組織が影響を受けるかどうかを調べます。</span><span class="sxs-lookup"><span data-stu-id="513d3-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="513d3-105">グローバル管理者と SharePoint 管理者には SharePoint のラインセンスが付与される必要があります。</span><span class="sxs-lookup"><span data-stu-id="513d3-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="513d3-106">新しく作成されたアカウントに SharePoint のライセンスまたは管理者の役割を割り当てた直後は、"アクセスが拒否されました" や "ユーザーが見つかりません" などのエラーが表示されて SharePoint にアクセスできない場合があります。</span><span class="sxs-lookup"><span data-stu-id="513d3-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="513d3-107">同期がシステム全体で完了するまで、少なくとも 24 時間お待ちください。</span><span class="sxs-lookup"><span data-stu-id="513d3-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="513d3-108">24 時間が長く感じられることは理解しております。</span><span class="sxs-lookup"><span data-stu-id="513d3-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="513d3-109">多くの場合、すでに解決策に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="513d3-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="513d3-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) ユーザーは、許可されたアクセス時間枠が小さすぎる場合に、アクセス拒否となる時があります。「[PIM アカウントに対するアクセスが拒否される](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="513d3-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>
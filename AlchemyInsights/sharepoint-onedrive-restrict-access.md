---
title: SharePoint または OneDrive でアクセスを制限する
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692770"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="099de-102">SharePoint または OneDrive でアクセスを制限する</span><span class="sxs-lookup"><span data-stu-id="099de-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="099de-103">SharePoint Online/OneDrive サービスへのアクセスを制限するさまざまな方法があります。</span><span class="sxs-lookup"><span data-stu-id="099de-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="099de-104">以降、これらのさまざまなアクセス制限方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="099de-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="099de-105">**アクセス許可の制限**</span><span class="sxs-lookup"><span data-stu-id="099de-105">**Permission Restriction**</span></span>

<span data-ttu-id="099de-106">SharePoint Online と OneDrive for Business で、アクセス権が必要なグループ/個人にのみアクセス権を付与することで、サイト、ファイル、フォルダーなどのアイテムへのアクセスを制限します。</span><span class="sxs-lookup"><span data-stu-id="099de-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="099de-107">SharePoint リストまたはライブラリのアクセス許可をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="099de-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="099de-108">SharePoint サイト権限をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="099de-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="099de-109">サブフォルダーの権限の変更</span><span class="sxs-lookup"><span data-stu-id="099de-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="099de-110">非管理対象デバイスからのアクセスを制御する</span><span class="sxs-lookup"><span data-stu-id="099de-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="099de-111">SharePoint またはグローバル管理者は、管理されていないデバイス (ハイブリッド AD に参加していないか、または Intune で準拠していないデバイス) からの SharePoint および OneDrive のコンテンツへのアクセスをブロックまたは制限することができます。</span><span class="sxs-lookup"><span data-stu-id="099de-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="099de-112">**ネットワークの場所の制限**</span><span class="sxs-lookup"><span data-stu-id="099de-112">**Network Location Restriction**</span></span>

<span data-ttu-id="099de-113">IT 管理者は、定義されている信頼できるネットワークの場所に基づいて、SharePoint と OneDrive のリソースへのアクセスを制御できます。</span><span class="sxs-lookup"><span data-stu-id="099de-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="099de-114">これは、場所に基づくポリシーとも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="099de-114">This is also known as location-based policy.</span></span> <span data-ttu-id="099de-115">詳細については、[「ネットワークの場所に基づいて SharePoint Online と OneDrive データへのアクセスを制御する」](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="099de-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="099de-116">**サイト ロックの制限**</span><span class="sxs-lookup"><span data-stu-id="099de-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="099de-117">SharePoint Online では、誰もアクセスできないようにサイト コレクションをロックできます。</span><span class="sxs-lookup"><span data-stu-id="099de-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="099de-118">これは、[Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState プロパティを使用して PowerShell および [SharePoint Online 管理シェル](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)を経由して設定されます。</span><span class="sxs-lookup"><span data-stu-id="099de-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="099de-119">**ユーザーがサイトまたはサブサイトを作成できないように制限する**</span><span class="sxs-lookup"><span data-stu-id="099de-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="099de-120">SharePoint 管理者またはグローバル管理者は、ユーザーが自分の SharePoint サイトを作成および管理したり、作成できるサイトの種類を決定したり、サイトの場所を指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="099de-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="099de-121">詳細については、[「SharePoint Online のサイト作成を管理する」](https://docs.microsoft.com/sharepoint/manage-site-creation)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="099de-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>


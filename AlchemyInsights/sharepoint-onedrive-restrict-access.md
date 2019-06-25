---
title: SharePoint または OneDrive でアクセスを制限する
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 3227f10270148c0e515b687c48058affa4d2be70
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35174473"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="4a73e-102">SharePoint または OneDrive でアクセスを制限する</span><span class="sxs-lookup"><span data-stu-id="4a73e-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="4a73e-103">SharePoint Online/OneDrive サービスへのアクセスを制限するには、さまざまな方法があります。</span><span class="sxs-lookup"><span data-stu-id="4a73e-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="4a73e-104">これらのさまざまなアクセス制限方法について、以下に説明します。</span><span class="sxs-lookup"><span data-stu-id="4a73e-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="4a73e-105">アクセス許可の制限</span><span class="sxs-lookup"><span data-stu-id="4a73e-105">Permission Restriction</span></span>

<span data-ttu-id="4a73e-106">SharePoint Online と OneDrive for business では、アクセスを必要とするグループまたは個人へのアクセスのみを許可することによって、サイト、ファイル、フォルダーなどのアイテムへのアクセスを制限します。</span><span class="sxs-lookup"><span data-stu-id="4a73e-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

[<span data-ttu-id="4a73e-107">SharePoint リストまたはライブラリのアクセス許可をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="4a73e-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[<span data-ttu-id="4a73e-108">SharePoint サイト権限をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="4a73e-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

[<span data-ttu-id="4a73e-109">サブフォルダーの権限の変更</span><span class="sxs-lookup"><span data-stu-id="4a73e-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[<span data-ttu-id="4a73e-110">非管理対象デバイスからのアクセスを制御する</span><span class="sxs-lookup"><span data-stu-id="4a73e-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="4a73e-111">Office 365 の SharePoint またはグローバル管理者は、管理されていないデバイス (ハイブリッド AD に参加していないか、または Intune で準拠していないデバイス) からの SharePoint および OneDrive のコンテンツへのアクセスをブロックまたは制限することができます。</span><span class="sxs-lookup"><span data-stu-id="4a73e-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="4a73e-112">ネットワークの場所の制限</span><span class="sxs-lookup"><span data-stu-id="4a73e-112">Network Location Restriction</span></span>

<span data-ttu-id="4a73e-113">IT 管理者は、信頼できる定義済みのネットワークの場所に基づいて SharePoint および OneDrive リソースへのアクセスを制御できます。</span><span class="sxs-lookup"><span data-stu-id="4a73e-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="4a73e-114">これは、場所ベースのポリシーとも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="4a73e-114">This is also known as location-based policy.</span></span> <span data-ttu-id="4a73e-115">詳細については、「[ネットワークの場所に基づいて SharePoint Online および OneDrive データへのアクセスを制御する](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a73e-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="4a73e-116">サイトロック制限</span><span class="sxs-lookup"><span data-stu-id="4a73e-116">Site Lock Restriction</span></span> 

<span data-ttu-id="4a73e-117">SharePoint Online では、サイトコレクションをロックダウンすることができます。アクセス権を持つユーザーはいません。</span><span class="sxs-lookup"><span data-stu-id="4a73e-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="4a73e-118">これは、PowerShell および[SharePoint Online 管理シェル](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)で[get-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState プロパティを使用して設定されます。</span><span class="sxs-lookup"><span data-stu-id="4a73e-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="4a73e-119">サイトまたはサブサイトの作成をユーザーに制限する</span><span class="sxs-lookup"><span data-stu-id="4a73e-119">Restrict users from creating sites or subsites</span></span>

<span data-ttu-id="4a73e-120">SharePoint 管理者または Office 365 のグローバル管理者は、ユーザーが自分の SharePoint サイトを作成および管理したり、作成できるサイトの種類を決定したり、サイトの場所を指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="4a73e-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="4a73e-121">詳細については、「 [SharePoint Online でサイト作成を管理](https://docs.microsoft.com/sharepoint/manage-site-creation)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a73e-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>


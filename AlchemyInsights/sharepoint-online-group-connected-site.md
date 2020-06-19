---
title: SharePoint サイトにグループを追加する
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582816"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="7d2de-102">SharePoint でグループ接続されたサイトを作成する際の問題</span><span class="sxs-lookup"><span data-stu-id="7d2de-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="7d2de-103">グループ接続されたサイトを作成または再作成する際に発生する一般的な問題がいくつかあります。</span><span class="sxs-lookup"><span data-stu-id="7d2de-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="7d2de-104">グループおよびグループと接続されたサイトを削除し、同じ URL で新たにサイトを作成する場合は、以前のサイトを完全に削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d2de-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="7d2de-105">[SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) をダウンロードする</span><span class="sxs-lookup"><span data-stu-id="7d2de-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="7d2de-106">PowerShell の使用を開始する方法の詳細については、「[SharePoint Online 管理シェルの使用を開始する](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d2de-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="7d2de-107">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell コマンドレットを使用して、削除されたサイトからサイトを削除します。</span><span class="sxs-lookup"><span data-stu-id="7d2de-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="7d2de-108">グループ サイトを完全に削除するには、PowerShell が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d2de-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="7d2de-109">グループ接続されたサイトを作成する際に、「**同じエイリアスのグループが既に存在しています**」という警告が表示される場合、[Microsoft 365 管理センター](https://admin.microsoft.com/AdminPortal/Home#/groups)で既存のグループを確認します。</span><span class="sxs-lookup"><span data-stu-id="7d2de-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="7d2de-110">この問題を解決するには、不要になった既存のグループを削除するか、異なるエイリアスを割り当ててサイトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7d2de-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="7d2de-111">SharePoint でモダン グループを作成および使用するには、さまざまな方法があります。</span><span class="sxs-lookup"><span data-stu-id="7d2de-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="7d2de-112">既存のサイトを Microsoft 365 グループに接続することができます。</span><span class="sxs-lookup"><span data-stu-id="7d2de-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="7d2de-113">詳細については、「[SharePoint ユーザー インターフェイスを使用して Microsoft 365 グループを接続する](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d2de-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="7d2de-114">Microsoft 365 のグループ接続されたサイトを作成するには、[チーム サイト](https://admin.microsoft.com/sharepoint)を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d2de-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>

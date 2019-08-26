---
title: SharePoint サイトにグループを追加する
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507852"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="570ba-102">SharePoint Online で接続されたサイトを作成またはグループ化する際の問題</span><span class="sxs-lookup"><span data-stu-id="570ba-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="570ba-103">グループ接続されたサイトを作成または再作成する際に発生する一般的な問題がいくつかあります。</span><span class="sxs-lookup"><span data-stu-id="570ba-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="570ba-104">グループおよびグループと接続されたサイトを削除し、同じ URL で新たにサイトを作成する場合は、以前のサイトを完全に削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="570ba-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="570ba-105">[SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) をダウンロードする</span><span class="sxs-lookup"><span data-stu-id="570ba-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="570ba-106">PowerShell の使用を開始する方法の詳細については、「[SharePoint Online 管理シェルの使用を開始する](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="570ba-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="570ba-107">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell コマンドレットを使用して、削除されたサイトからサイトを削除します。</span><span class="sxs-lookup"><span data-stu-id="570ba-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="570ba-108">グループ接続されたサイトを作成する際に、同じエイリアスのグループが既に存在していますという警告が表示される場合、[Office 365 管理センター](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)で既存のグループを確認します。</span><span class="sxs-lookup"><span data-stu-id="570ba-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="570ba-109">この問題を解決するには、不要になった既存のグループを削除するか、異なるエイリアスを割り当ててサイトを作成します。</span><span class="sxs-lookup"><span data-stu-id="570ba-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="570ba-110">SharePoint でモダン グループを作成および使用するには、さまざまな方法があります。</span><span class="sxs-lookup"><span data-stu-id="570ba-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="570ba-111">既存のサイトを Office 365 グループに接続することができます。</span><span class="sxs-lookup"><span data-stu-id="570ba-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="570ba-112">詳細については、「[SharePoint ユーザー インターフェイスを使用して Office 365 グループを接続する](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="570ba-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="570ba-113">Office 365 のグループ接続されたサイトを作成するには、チーム サイトを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="570ba-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="570ba-114">詳細については、「[SharePoint Online でチーム サイトを作成する](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="570ba-114">For more info, see [Delete a site in the new SharePoint admin center](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>


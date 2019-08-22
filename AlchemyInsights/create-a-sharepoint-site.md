---
title: SharePoint サイトを作成する
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 96780bd2f4182c1385406ec2a31cd62745137985
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515812"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="91ea6-102">SharePoint サイトを作成する</span><span class="sxs-lookup"><span data-stu-id="91ea6-102">Create a SharePoint site</span></span>

<span data-ttu-id="91ea6-103">SharePoint サイトの作成の詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91ea6-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="91ea6-104">[新しい SharePoint 管理センターでサイトを管理](https://docs.microsoft.com/sharepoint/manage-site-creation)する: 従来のサイトを作成する方法や、Office 365 グループを含まない teams サイトを作成する方法など、サイト作成オプションについて説明します。</span><span class="sxs-lookup"><span data-stu-id="91ea6-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="91ea6-105">[SharePoint でチームサイトを作成](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US)する: チームサイトを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="91ea6-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="91ea6-106">[SharePoint Online でコミュニケーションサイトを作成](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)する: コミュニケーションサイトを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="91ea6-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="91ea6-107">[新しい SharePoint 管理センターでサイトを管理](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site)する: Office 365 グループを含まない従来のサイトまたはチームサイトを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="91ea6-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="91ea6-108">[!記載</span><span class="sxs-lookup"><span data-stu-id="91ea6-108">[!Tips]</span></span>
> - <span data-ttu-id="91ea6-109">既存のサイトの同じ URL を持つサイトを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="91ea6-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="91ea6-110">サイトを削除して URL を再利用したい場合は、削除されたサイトが**削除済み**サイトの下に存在する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="91ea6-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="91ea6-111">削除されたサイトを管理するには、「[サイトを削除する](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91ea6-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="91ea6-112">PowerShell を使ってサイトを完全に削除するには、[Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) コマンドレットの例を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91ea6-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="91ea6-113">ユーザーによっては、サイトを作成できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="91ea6-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="91ea6-114">「 [SharePoint Online でサイト作成を管理](https://docs.microsoft.com/sharepoint/manage-site-creation)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91ea6-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="91ea6-115">サイトが予想より長く**作成**されているように見えることがあります。</span><span class="sxs-lookup"><span data-stu-id="91ea6-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="91ea6-116">この問題が最初に発生してから24時間以上経過している場合は、サポートチケットをログに記録してください。</span><span class="sxs-lookup"><span data-stu-id="91ea6-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="91ea6-117">多くの場合、すでに解決策に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="91ea6-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="91ea6-118">解決策を完成させるために少なくとも 24 時間を与えてください。</span><span class="sxs-lookup"><span data-stu-id="91ea6-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="91ea6-119">Office 365 グループを含まない新しいチームサイトを作成する必要がある場合は、</span><span class="sxs-lookup"><span data-stu-id="91ea6-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 



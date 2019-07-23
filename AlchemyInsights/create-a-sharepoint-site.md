---
title: SharePoint サイトを作成する
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802971"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="9f6f8-102">SharePoint サイトを作成する</span><span class="sxs-lookup"><span data-stu-id="9f6f8-102">Create a SharePoint site</span></span>

<span data-ttu-id="9f6f8-103">SharePoint サイト作成の詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="9f6f8-104">[新しい SharePoint 管理センターでサイトを管理する](https://docs.microsoft.com/sharepoint/manage-site-creation): Office 365 グループを含まない従来のサイトやチーム サイトの作成方法など、サイト作成のオプションを参照することができます。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="9f6f8-105">[SharePoint でチーム サイトを作成する](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): チーム サイトの作成方法を参照することができます。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="9f6f8-106">[SharePoint Online でコミュニケーション サイトを作成する](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): コミュニケーション サイトの作成方法を参照することができます。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="9f6f8-107">[新しい SharePoint 管理センターでサイトを管理する](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Office 365 グループを含まない従来のサイトやチーム サイトの作成方法を参照することができます。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-107">See Manage sites in the new SharePoint admin center for site creation options. Select to create a team site (which will create an Office 365 group) or a communication site. To create a classic site, or a new team site that doesn't include an Office 365 group, click Other options.</span></span>


  
> <span data-ttu-id="9f6f8-108">ヒント</span><span class="sxs-lookup"><span data-stu-id="9f6f8-108">Tips</span></span>
> - <span data-ttu-id="9f6f8-109">既存のサイトと同じ URL のサイトを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-109">Note: You cannot create a new site that has the same URL with an existing site.</span></span> <span data-ttu-id="9f6f8-110">サイトを削除し、その URL を再利用する場合は、削除したサイトがまだ **[削除されたサイト]** の下に存在している場合があります。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="9f6f8-111">削除したサイトを管理するには、「[サイトを削除する](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="9f6f8-112">PowerShell を使ってサイトを完全に削除するには、[Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) コマンドレットの例を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="9f6f8-113">一部のユーザーはサイトを作成できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-113">Some users may not be able to create a site. See Manage site creation in SharePoint Online.</span></span> <span data-ttu-id="9f6f8-114">その場合は、「[SharePoint Online のサイト作成を管理する](https://docs.microsoft.com/sharepoint/manage-site-creation)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-114">[Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>
> - <span data-ttu-id="9f6f8-115">サイトの**作成中**に、サイトが予想以上に長く停止しているように見えることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="9f6f8-116">この問題が発生してから 24 時間以上経過した場合は、サポート チケットを記録してください。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="9f6f8-117">多くの場合、すでに解決策に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="9f6f8-118">解決策を完成させるために少なくとも 24 時間を与えてください。</span><span class="sxs-lookup"><span data-stu-id="9f6f8-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="9f6f8-119">Office 365 グループを含まない新しいチーム サイトを作成する場合は、</span><span class="sxs-lookup"><span data-stu-id="9f6f8-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 



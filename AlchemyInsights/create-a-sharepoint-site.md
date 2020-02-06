---
title: SharePoint サイトを作成する
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770860"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="b8b58-102">SharePoint サイトを作成する</span><span class="sxs-lookup"><span data-stu-id="b8b58-102">Create a SharePoint site</span></span>

<span data-ttu-id="b8b58-103">SharePoint 管理センターで[アクティブなサイト](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true)からサイトを作成または管理します。</span><span class="sxs-lookup"><span data-stu-id="b8b58-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="b8b58-104">詳細については、「[新しい SharePoint 管理センターでサイトを管理する](https://docs.microsoft.com/sharepoint/manage-site-creation)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8b58-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="b8b58-105">ヒント:</span><span class="sxs-lookup"><span data-stu-id="b8b58-105">Tips:</span></span>

- <span data-ttu-id="b8b58-106">既存のサイトと同じ URL のサイトを作成することは**できません**。</span><span class="sxs-lookup"><span data-stu-id="b8b58-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="b8b58-107">サイトを削除し、その URL を再利用する場合は、削除したサイトがまだ [[削除されたサイト](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)] の下に存在している場合があります。</span><span class="sxs-lookup"><span data-stu-id="b8b58-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="b8b58-108">URL を再利用するには、サイトを完全に削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b8b58-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="b8b58-109">PowerShell を使ってサイトを完全に削除するには、[Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) コマンドレットの例を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8b58-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="b8b58-110">一部のユーザーはサイトを作成できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="b8b58-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="b8b58-111">「[SharePoint Online のサイト作成を管理する](https://docs.microsoft.com/sharepoint/manage-site-creation)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8b58-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="b8b58-112">サイトの**作成中**に、サイトが予想以上に長く停止しているように見えることがあります。</span><span class="sxs-lookup"><span data-stu-id="b8b58-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="b8b58-113">この問題が発生してから 24 時間以上経過した場合は、サポート チケットを記録してください。</span><span class="sxs-lookup"><span data-stu-id="b8b58-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="b8b58-114">多くの場合、すでに解決策に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="b8b58-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b8b58-115">解決策を完成させるために少なくとも 24 時間を与えてください。</span><span class="sxs-lookup"><span data-stu-id="b8b58-115">Please give us at least 24 hours to complete a solution.</span></span>

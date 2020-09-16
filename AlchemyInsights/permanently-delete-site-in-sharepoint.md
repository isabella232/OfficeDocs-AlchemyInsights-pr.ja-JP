---
title: SharePoint のサイトを完全に削除する
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771726"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="a8e12-102">SharePoint のサイトを完全に削除する</span><span class="sxs-lookup"><span data-stu-id="a8e12-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="a8e12-103">(サイトを再作成するために) 削除したサイトの URL を再利用する場合、または使用しなくなったサイトを完全に削除する場合には、新しい SharePoint 管理センターの **[完全に削除]** を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a8e12-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="a8e12-104">[新しい SharePoint 管理センターの [削除されたサイト] ページ](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)に移動し、組織の管理者権限が付与されているアカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="a8e12-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="a8e12-105">左側の列で、サイトをクリックします。</span><span class="sxs-lookup"><span data-stu-id="a8e12-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="a8e12-106">**[完全に削除]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a8e12-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="a8e12-107">**注**: 新しい SharePoint 管理センターからは、グループが接続されているサイトを完全に削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="a8e12-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="a8e12-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) を代わりに使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a8e12-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="a8e12-109">詳しくは、「[サイトを完全に削除する](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8e12-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 

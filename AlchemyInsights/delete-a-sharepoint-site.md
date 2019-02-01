---
title: SharePoint サイトを削除する
ms.author: kirks
author: Techwriter40
ms.date: 1/24/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: c060815d-1d3f-4a13-81c2-0377bbeda202
ms.openlocfilehash: ddedfff905b4f3eb78cdd8b17233d45f864dadd4
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660021"
---
# <a name="delete-a-sharepoint-site"></a><span data-ttu-id="efd9f-102">SharePoint サイトを削除する</span><span class="sxs-lookup"><span data-stu-id="efd9f-102">Delete a SharePoint site</span></span>
 <span data-ttu-id="efd9f-103">**新しい SharePoint 管理センターからサイトを削除する**</span><span class="sxs-lookup"><span data-stu-id="efd9f-103">**Delete sites from the new SharePoint admin center**</span></span>
  
<span data-ttu-id="efd9f-p101">アクティブなサイトを削除するには、現在の SharePoint 管理センターに移動して、右上で [今すぐ使ってみる] をクリックします。[**アクティブなサイト**] を選択してそのサイトを選び、[**削除**] を選択します。[新しい SharePoint 管理センターで削除されたサイトを表示または復元する](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center)には、[**削除されたサイト**] を選択します。詳細については、「[新しい SharePoint 管理センターのサイトを管理する](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efd9f-p101">To delete an active site, go to the current SharePoint admin center, click "Try it now" in the upper right. Select **Active sites**, select the site, and then select **Delete**. To [view and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center), select **Deleted sites**. For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center).</span></span>
  
<span data-ttu-id="efd9f-p102">**重要:** サイトがアイテム保持ポリシーの一部である場合は、[セキュリティ&amp;コンプライアンス管理センター](https://protection.office.com/?rfr=AdminCenter#/homepage)からそのサイトが削除されるまで、サイトを削除できない場合があります。詳細については、「[アイテム保持ポリシーの概要](https://docs.microsoft.com/office365/securitycompliance/retention-policies#content-in-onedrive-accounts-and-sharepoint-sites)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efd9f-p102">**Important:** If the site is part of a retention policy, you may not be able to delete it until the site is removed from the [Security &amp; Compliance Admin Center](https://protection.office.com/?rfr=AdminCenter#/homepage). See [Overview of Retention Policies](https://docs.microsoft.com/office365/securitycompliance/retention-policies#content-in-onedrive-accounts-and-sharepoint-sites) for more info.</span></span> 
  
<span data-ttu-id="efd9f-110">ヒント:</span><span class="sxs-lookup"><span data-stu-id="efd9f-110">Tips</span></span>
- <span data-ttu-id="efd9f-p103">グローバル管理者と SharePoint 管理者は、**Office 365 グループ**に属しているサイトを削除できるようになりました。これにより、グループとそのグループのすべてのリソース (Outlook メールボックス、予定表、Teams チャンネルなど) が削除されます。詳細については、[SharePoint サイトの削除](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="efd9f-p103">Global admins and SharePoint admins can now delete sites that belong to an **Office 365 Group**. This will delete the group and all its resources, including the Outlook mailbox and calendar, and any Teams channels. For more info, see [Delete a SharePoint site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span></span>
- <span data-ttu-id="efd9f-p104">削除されたサイトは 93 日間復元できます。削除されたグループは 30 日以内に復元する必要があります。詳細については、[削除されたサイトの表示と復元](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="efd9f-p104">You can recover deleted sites for 93 days. Note that deleted groups must be restored within 30 days. For more info, see [View and restore deleted sites](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center).</span></span>
- <span data-ttu-id="efd9f-117">PowerShell を使ってサイトを完全に削除するには、[Remove-SPSite](https://docs.microsoft.com/powershell/module/sharepoint-server/remove-spsite?view=sharepoint-ps) コマンドレットの例を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efd9f-117">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/powershell/module/sharepoint-server/remove-spsite?view=sharepoint-ps) cmdlet example.</span></span> 
  


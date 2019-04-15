---
title: 外部ユーザーと共有できない
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747603"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="e28fe-102">外部ユーザーと SharePoint コンテンツを共有できない問題を修正する</span><span class="sxs-lookup"><span data-stu-id="e28fe-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="e28fe-103">組織の外部共有がオンになっていることを確認する:</span><span class="sxs-lookup"><span data-stu-id="e28fe-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="e28fe-104">Microsoft 365 管理センターで、[[サービスとアドイン]](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns) ページに移動して、**[サイト]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="e28fe-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="e28fe-p101">設定が "オン" になっていることを確認します。"既存の外部ユーザーのみ" が選択されている場合、Microsoft 365 管理センターのリストに外部ユーザーが表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="e28fe-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="e28fe-p102">サイトに対して外部共有がオンになっていることを確認します。従来のサイト コレクションの場合:</span><span class="sxs-lookup"><span data-stu-id="e28fe-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="e28fe-109">新しい SharePoint 管理センターの左側のウィンドウで、**[サイト]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e28fe-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="e28fe-110">サイトを選択し、リボンで [**共有**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="e28fe-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="e28fe-111">Office 365 グループに属するチーム サイトの場合とコミュニケーション サイトの場合:</span><span class="sxs-lookup"><span data-stu-id="e28fe-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="e28fe-p103">サインインを要求しないリンクを利用したファイル共有が組織全体の設定で許可されている場合を除き、この新しい種類のサイトには組織全体の設定と同じ共有設定が与えられます。サイトでは、サインインした新しい外部ユーザーと既存外部ユーザーとの共有が許可されます。特定のサイトの設定を変更するには、新しい SharePoint 管理センターまたは PowerShell を使用します。詳細は[こちら](https://go.microsoft.com/fwlink/?linkid=871863)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e28fe-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="e28fe-116">サイトの外部共有設定には、組織全体設定の場合より制限を増やすことができますが、組織全体設定の場合より制限を減らすことはできません。</span><span class="sxs-lookup"><span data-stu-id="e28fe-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  


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
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4b132a3cb0fac015ab44a1fa08565af15b7e8121
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207690"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="65ef6-102">外部ユーザーと SharePoint コンテンツを共有できない問題を修正する</span><span class="sxs-lookup"><span data-stu-id="65ef6-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="65ef6-103">組織の外部共有がオンになっていることを確認する:</span><span class="sxs-lookup"><span data-stu-id="65ef6-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="65ef6-104">Microsoft 365 管理センターで、[[サービスとアドイン]](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns) ページに移動して、**[サイト]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="65ef6-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="65ef6-p101">設定が "オン" になっていることを確認します。"既存の外部ユーザーのみ" が選択されている場合、Microsoft 365 管理センターのリストに外部ユーザーが表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="65ef6-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="65ef6-p102">サイトに対して外部共有がオンになっていることを確認します。従来のサイト コレクションの場合:</span><span class="sxs-lookup"><span data-stu-id="65ef6-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="65ef6-109">従来の SharePoint 管理センターで、左のウィンドウにある [**サイト コレクション**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="65ef6-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="65ef6-110">サイトを選択し、リボンで [**共有**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="65ef6-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="65ef6-111">Office 365 グループに属するチーム サイトの場合とコミュニケーション サイトの場合:</span><span class="sxs-lookup"><span data-stu-id="65ef6-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="65ef6-p103">サインインを要求しないリンクを利用したファイル共有が組織全体の設定で許可されている場合を除き、この新しい種類のサイトには組織全体の設定と同じ共有設定が与えられます。サイトでは、サインインした新しい外部ユーザーと既存外部ユーザーとの共有が許可されます。特定のサイトの設定を変更するには、新しい SharePoint 管理センター (プレビュー) または PowerShell を使用します。詳細は[こちら](https://go.microsoft.com/fwlink/?linkid=871863)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="65ef6-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="65ef6-116">サイトの外部共有設定には、組織全体設定の場合より制限を増やすことができますが、組織全体設定の場合より制限を減らすことはできません。</span><span class="sxs-lookup"><span data-stu-id="65ef6-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  


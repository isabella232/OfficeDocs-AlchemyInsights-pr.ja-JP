---
title: 外部ユーザーと共有できない
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582780"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>外部ユーザーと SharePoint コンテンツを共有できない問題を修正する

組織の外部共有がオンになっていることを確認する:
  
1. Microsoft 365 管理センターで、[[サービスとアドイン]](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns) ページに移動して、**[サイト]** をクリックします。
    
2. Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.
    
Make sure external sharing it turned on for the site. For a classic site collection:
  
1. 新しい SharePoint 管理センターの左側のウィンドウで、**[サイト]** を選択します。
    
2. サイトを選択し、リボンで [**共有**] をクリックします。
    
Microsoft 365 グループに属するチーム サイトの場合とコミュニケーション サイトの場合:
  
- These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> サイトの外部共有設定には、組織全体設定の場合より制限を増やすことができますが、組織全体設定の場合より制限を減らすことはできません。 
  


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
ms.openlocfilehash: 700e6d24e49cf11bf91780895f5a796cc1d8349d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753431"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>外部ユーザーと SharePoint コンテンツを共有できない問題を修正する

組織の外部共有がオンになっていることを確認する:
  
1. Microsoft 365 管理センターで、[[サービスとアドイン]](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns) ページに移動して、**[サイト]** をクリックします。
    
2. 設定が "オン" になっていることを確認します。"既存の外部ユーザーのみ" が選択されている場合、Microsoft 365 管理センターのリストに外部ユーザーが表示されていることを確認します。
    
サイトに対して外部共有がオンになっていることを確認します。従来のサイト コレクションの場合:
  
1. 従来の SharePoint 管理センターで、左のウィンドウにある [**サイト コレクション**] をクリックします。
    
2. サイトを選択し、リボンで [**共有**] をクリックします。
    
Office 365 グループに属するチーム サイトの場合とコミュニケーション サイトの場合:
  
- サインインを要求しないリンクを利用したファイル共有が組織全体の設定で許可されている場合を除き、この新しい種類のサイトには組織全体の設定と同じ共有設定が与えられます。サイトでは、サインインした新しい外部ユーザーと既存外部ユーザーとの共有が許可されます。特定のサイトの設定を変更するには、新しい SharePoint 管理センター (プレビュー) または PowerShell を使用します。詳細は[こちら](https://go.microsoft.com/fwlink/?linkid=871863)をご覧ください。
    
> [!NOTE]
> サイトの外部共有設定には、組織全体設定の場合より制限を増やすことができますが、組織全体設定の場合より制限を減らすことはできません。 
  


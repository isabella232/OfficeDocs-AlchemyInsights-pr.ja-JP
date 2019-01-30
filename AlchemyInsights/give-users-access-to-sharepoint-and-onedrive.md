---
title: SharePoint と OneDrive へのアクセス権をユーザーに付与する
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 5a1cdeefa4474e8ce0e6a7a37be016cc87b9791d
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498019"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="565bd-102">SharePoint と OneDrive へのアクセス権をユーザーに付与する</span><span class="sxs-lookup"><span data-stu-id="565bd-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="565bd-p101">OneDrive または SharePoint サイトがアクセス権を持っている複数のユーザーから利用できない場合は、一時的なサービス上の問題が発生している可能性があります。[サービス正常性ダッシュボードを確認する](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="565bd-p101">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue. [Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth)</span></span>
  
<span data-ttu-id="565bd-p102">組織内のユーザーが SharePoint と OneDrive にサインインして使用できるようにするには、そのためのアカウントを追加して、SharePoint と OneDrive へのアクセス権を付与するライセンスがあるかどうかを確認する必要があります。ユーザーを追加する最も簡単な方法が Office 365 管理センター内にあります。</span><span class="sxs-lookup"><span data-stu-id="565bd-p102">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive. The easiest way to add users is in the Office 365 admin center.</span></span>
  
1. <span data-ttu-id="565bd-107">[Office 365 管理センターで [アクティブ ユーザー] ページ](https://portal.office.com/adminportal/home#/users)に移動してから、**[ユーザーの追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="565bd-107">Go to the [Active users page in the Office 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="565bd-108">ユーザーに関する情報を入力して、**[製品のライセンス]** で、ライセンスが割り当てられており、**[SharePoint Online]** が選択されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="565bd-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="565bd-p103">組織内で外部共有を許可すると、ユーザーが SharePoint と OneDrive のコンテンツを組織外部のユーザーと共有できることに注意してください。このような外部ユーザーにライセンスを付与する必要はありません。また、共有が [既存の外部ユーザーのみ] に設定されていなければ、彼ら用のアカウントを追加する必要もありません。共有がそのように設定されている場合は、ユーザーが組織内のディレクトリに存在しなければ、Azure AD 管理センターで彼らをゲスト ユーザーとして追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="565bd-p103">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization. You don't need to give these external users licenses. You also don't need to add accounts for them, unless sharing is set to "Only existing external users." In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  


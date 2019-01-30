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
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>SharePoint と OneDrive へのアクセス権をユーザーに付与する

> [!NOTE]
> OneDrive または SharePoint サイトがアクセス権を持っている複数のユーザーから利用できない場合は、一時的なサービス上の問題が発生している可能性があります。[サービス正常性ダッシュボードを確認する](https://portal.office.com/adminportal/home#/servicehealth)
  
組織内のユーザーが SharePoint と OneDrive にサインインして使用できるようにするには、そのためのアカウントを追加して、SharePoint と OneDrive へのアクセス権を付与するライセンスがあるかどうかを確認する必要があります。ユーザーを追加する最も簡単な方法が Office 365 管理センター内にあります。
  
1. [Office 365 管理センターで [アクティブ ユーザー] ページ](https://portal.office.com/adminportal/home#/users)に移動してから、**[ユーザーの追加]** をクリックします。
    
2. ユーザーに関する情報を入力して、**[製品のライセンス]** で、ライセンスが割り当てられており、**[SharePoint Online]** が選択されていることを確認します。 
    
組織内で外部共有を許可すると、ユーザーが SharePoint と OneDrive のコンテンツを組織外部のユーザーと共有できることに注意してください。このような外部ユーザーにライセンスを付与する必要はありません。また、共有が [既存の外部ユーザーのみ] に設定されていなければ、彼ら用のアカウントを追加する必要もありません。共有がそのように設定されている場合は、ユーザーが組織内のディレクトリに存在しなければ、Azure AD 管理センターで彼らをゲスト ユーザーとして追加する必要があります。
  


---
title: SharePoint と OneDrive へのアクセス権をユーザーに付与する
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 1be9763ce7766c6261f0c1dae78ced6727c7a88d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "36523768"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>SharePoint と OneDrive へのアクセス権をユーザーに付与する

> [!NOTE]
> OneDrive または SharePoint サイトがアクセス権を持っている複数のユーザーから利用できない場合は、一時的なサービス上の問題が発生している可能性があります。[サービス正常性ダッシュボードを確認する](https://portal.office.com/adminportal/home#/servicehealth)
  
組織内のユーザーが SharePoint と OneDrive にサインインして使用できるようにするには、そのためのアカウントを追加して、SharePoint と OneDrive へのアクセス権を付与するライセンスがあるかどうかを確認する必要があります。ユーザーを追加する最も簡単な方法が Microsoft 365 管理センター内にあります。
  
1. [Microsoft 365 管理センターで [アクティブなユーザー] ページ](https://portal.office.com/adminportal/home#/users)に移動してから、**[ユーザーの追加]** をクリックします。
    
2. ユーザーに関する情報を入力して、**[製品のライセンス]** で、ライセンスが割り当てられており、**[SharePoint Online]** が選択されていることを確認します。 
    
組織内で外部共有を許可すると、ユーザーが SharePoint と OneDrive のコンテンツを組織外部のユーザーと共有できることに注意してください。このような外部ユーザーにライセンスを付与する必要はありません。また、共有が [既存の外部ユーザーのみ] に設定されていなければ、彼ら用のアカウントを追加する必要もありません。共有がそのように設定されている場合は、ユーザーが組織内のディレクトリに存在しなければ、Azure AD 管理センターで彼らをゲスト ユーザーとして追加する必要があります。
  


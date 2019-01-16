---
title: プロファイルの同期
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297662"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="ace53-102">SharePoint ユーザー プロファイル アプリケーションを自分のプロファイルの変更内容の同期と</span><span class="sxs-lookup"><span data-stu-id="ace53-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="ace53-103">SharePoint Online は、ユーザー プロファイル アプリケーションにユーザーとグループをインポートするのには Active Directory のインポートのタイマー ジョブ (AD のインポート) を使用します。</span><span class="sxs-lookup"><span data-stu-id="ace53-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="ace53-p101">AD のインポートでは、SharePoint のオンライン ディレクトリ ストアからユーザー プロファイル アプリケーションへの変更を同期します。これらの変更は、バッチで処理されます。</span><span class="sxs-lookup"><span data-stu-id="ace53-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="ace53-106">変更が同期されるまで、タイマー ジョブが実行されます。</span><span class="sxs-lookup"><span data-stu-id="ace53-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="ace53-p102">ジョブの実行にかかる時間は、変更を処理するための数によって異なります。多数の変更に時間がかかります。サービス レベル契約 (SLA) では、SharePoint のオンライン ディレクトリ内のユーザーへの変更を 24 時間でのユーザー プロファイル アプリケーションに反映されることを示しています。</span><span class="sxs-lookup"><span data-stu-id="ace53-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="ace53-110">SharePoint Online でユーザー プロファイルの同期に関する詳細情報</span><span class="sxs-lookup"><span data-stu-id="ace53-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  


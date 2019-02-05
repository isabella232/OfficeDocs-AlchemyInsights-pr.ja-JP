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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477436"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="7031e-102">自分のプロファイルの変更は、SharePoint ユーザー プロファイル アプリケーションに同期されますか。</span><span class="sxs-lookup"><span data-stu-id="7031e-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="7031e-103">SharePoint Online では、Active Directory Import タイマー ジョブ (AD Import) を使用して、ユーザーとグループをユーザー プロファイル アプリケーションにインポートします。</span><span class="sxs-lookup"><span data-stu-id="7031e-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="7031e-p101">変更は AD Import によって SharePoint Online のディレクトリ ストアからユーザー プロファイル アプリケーションに同期されます。これらの変更は一括で処理されます。</span><span class="sxs-lookup"><span data-stu-id="7031e-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="7031e-106">タイマー ジョブは、変更が同期されるまで実行されます。</span><span class="sxs-lookup"><span data-stu-id="7031e-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="7031e-p102">ジョブの実行にかかる時間は処理する変更の数によって異なります。変更の数が多いと、時間も長くなります。サービス レベル アグリーメント (SLA) では、SharePoint Online ディレクトリでのユーザーに対する変更は 24 時間でユーザー プロファイル アプリケーションに反映されるものと規定されています。</span><span class="sxs-lookup"><span data-stu-id="7031e-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="7031e-110">SharePoint Online でのユーザープロファイルの同期に関する詳細情報</span><span class="sxs-lookup"><span data-stu-id="7031e-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  


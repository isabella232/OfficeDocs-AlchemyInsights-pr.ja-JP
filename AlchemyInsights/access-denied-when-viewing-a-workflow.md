---
title: ワークフローを表示するとき、アクセスが拒否されました
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297352"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="3e8bb-102">ワークフローを表示するとき、アクセスが拒否されました</span><span class="sxs-lookup"><span data-stu-id="3e8bb-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="3e8bb-103">SharePoint グループに電子メールを送信しようとする SharePoint 2013 ワークフローは SharePoint グループのメンバーシップは、すべてのユーザーに設定されていない場合"アクセスが拒否されました"というエラー メッセージが失敗します。</span><span class="sxs-lookup"><span data-stu-id="3e8bb-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="3e8bb-104">**この問題を解決するには、次の手順を行います。**</span><span class="sxs-lookup"><span data-stu-id="3e8bb-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="3e8bb-105">SharePoint グループのメンバーを表示するのにはすべてのユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="3e8bb-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="3e8bb-106">SharePoint グループから削除] または [cc] 行の電子メールです。</span><span class="sxs-lookup"><span data-stu-id="3e8bb-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="3e8bb-107">明示的にユーザーを追加] または [cc] 行の場合は、SharePoint グループのメンバーシップの表示/非表示を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="3e8bb-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="3e8bb-108">表示するには、詳細についてを参照してください[/_vti_bin/client.svc/sp.utilities.utility.SendEmail する HTTP 承認されていません](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)。</span><span class="sxs-lookup"><span data-stu-id="3e8bb-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  


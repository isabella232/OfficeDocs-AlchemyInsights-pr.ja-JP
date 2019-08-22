---
title: ワークフローを表示しようとするとアクセスが拒否される
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495828"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="e0656-102">ワークフローを表示しようとするとアクセスが拒否される</span><span class="sxs-lookup"><span data-stu-id="e0656-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="e0656-103">SharePoint グループのメンバーシップがすべてのユーザーに設定されていないと、SharePoint グループにメールを送信する SharePoint 2013 ワークフローを表示しようとする際に「アクセスが拒否されました」というエラー メッセージが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e0656-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="e0656-104">**この問題を解決するには、次の操作を行います。**</span><span class="sxs-lookup"><span data-stu-id="e0656-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="e0656-105">すべてのユーザーに SharePoint グループのメンバーが表示されるようにします。</span><span class="sxs-lookup"><span data-stu-id="e0656-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="e0656-106">メールの宛先または CC 行から SharePoint グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="e0656-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="e0656-107">SharePoint グループのメンバーシップの表示設定を変更できない場合は、To または CC 行にユーザーを明示的に追加します。</span><span class="sxs-lookup"><span data-stu-id="e0656-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="e0656-108">詳細を表示するには、 [/_vti_bin/client.svc/sp.utilities.utility.SendEmail に対する承認されていない HTTP](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0656-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  
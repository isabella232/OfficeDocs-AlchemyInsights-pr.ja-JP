---
title: ワークフローを表示しようとするとアクセスが拒否される
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687335"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="ecaea-102">ワークフローを表示しようとするとアクセスが拒否される</span><span class="sxs-lookup"><span data-stu-id="ecaea-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="ecaea-103">SharePoint グループのメンバーシップがすべてのユーザーに設定されていないと、SharePoint グループにメールを送信する SharePoint 2013 ワークフローを表示しようとする際に「アクセスが拒否されました」というエラー メッセージが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ecaea-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="ecaea-104">**この問題を解決するには、次の操作を行います。**</span><span class="sxs-lookup"><span data-stu-id="ecaea-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="ecaea-105">すべてのユーザーに SharePoint グループのメンバーが表示されるようにします。</span><span class="sxs-lookup"><span data-stu-id="ecaea-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="ecaea-106">メールの宛先または CC 行から SharePoint グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="ecaea-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="ecaea-107">SharePoint グループのメンバーシップの表示設定を変更できない場合は、To または CC 行にユーザーを明示的に追加します。</span><span class="sxs-lookup"><span data-stu-id="ecaea-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="ecaea-108">詳細については「[/_vti_bin/client.svc/sp.utilities.utility.SendEmail への HTTP 権限エラー](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ecaea-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  
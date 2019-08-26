---
title: 125 Outlook on the web で無効なライセンス エラーが表示される場合
ms.author: daeite
author: daeite
manager: jackiesm
ms.date: 4/9/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "125"
- "1600021"
ms.assetid: 6d9947d9-6c92-4ada-b655-8ab2a0c2b66d
ms.openlocfilehash: d0f3fa354eb63c5a5f92d017694623c36fc6df30
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36523804"
---
# <a name="getting-an-invalid-license-error-in-outlook-on-the-web"></a><span data-ttu-id="2daf4-102">Outlook on the web で無効なライセンス エラーが表示される場合</span><span class="sxs-lookup"><span data-stu-id="2daf4-102">Getting an invalid license error in Outlook on the web?</span></span>

<span data-ttu-id="2daf4-p101">Outlook on the web を使用しているときに、**X-OWA-Error: Microsoft.Exchange.Data.Storage.InvalidLicenseException** を含む "**問題が発生しました**" エラーが表示される場合は、Exchange Online ライセンスが正しく割り当てられていないか、最近有効期限が切れています。管理者は、以下の手順に従うことで、ライセンスを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="2daf4-p101">If you're using Outlook on the web and you get a **Something went wrong** error that contains **X-OWA-Error: Microsoft.Exchange.Data.Storage.InvalidLicenseException**, your Exchange Online license isn't correctly assigned or has recently expired. Your admin can assign a license to you by following these steps:</span></span>
  
1. <span data-ttu-id="2daf4-105">[Microsoft 365 管理センター](https://portal.office.com/adminportal/home#/homepage)を開いて、**[アクティブなユーザー]** で、**[ユーザーの編集]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2daf4-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and under **Active users**, select **Edit a user**.</span></span>

2. <span data-ttu-id="2daf4-p102">開いた **[ユーザーの編集]** ページで、ユーザーを選択します。開いた [ユーザーのプロパティ] ページで、**[製品のライセンス]** の **[編集]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="2daf4-p102">In the **Edit a user** page that opens, select the user. In the user properties page that opens, click **Edit** for **Product licenses**.</span></span>

3. <span data-ttu-id="2daf4-p103">開いた **[製品のライセンス]** ページで、該当する **[場所]** の値を選択し、Exchange Online を含むライセンスを割り当てます (ライセンスを展開して、その詳細を表示します)。完了したら、**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="2daf4-p103">In the **Product licenses** page that opens, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details). When you're finished, click **Save**.</span></span>

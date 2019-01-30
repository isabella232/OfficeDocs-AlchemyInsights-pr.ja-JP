---
title: 126 OWA で「メールボックスが見つかりませんでした」というエラーが表示される場合
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 4/9/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6ef8a706ac14d6b1c11c467800e0c41df2450ea1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477593"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="50b98-102">Outlook on the web で「メールボックスが見つかりませんでした」というエラーが表示される場合</span><span class="sxs-lookup"><span data-stu-id="50b98-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="50b98-p101">Outlook on the web を使用しているときに、「**メールボックスが見つかりませんでした**」というエラーが表示された場合は、Outlook on the web への接続時に使用したアカウントに Exchange Online ライセンスが付与されていないため、そのアカウントにメールボックスが関連付けられていません。管理者は、次の手順に従ってアカウントにライセンスを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="50b98-p101">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account. Your admin can assign a license to your account by following these steps:</span></span> 
  
1. <span data-ttu-id="50b98-105">[Office 365 管理センター](https://portal.office.com/adminportal/home#/homepage)を開いて、**[アクティブなユーザー]** で、**[ユーザーの編集]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="50b98-105">Open the [Office 365 admin center](https://portal.office.com/adminportal/home#/homepage) and under **Active users**, select **Edit a user**.</span></span>
    
2. <span data-ttu-id="50b98-p102">表示された **[ユーザーの編集]** ページで、ユーザーを選択します。表示された [ユーザーのプロパティ] ページで、**[製品のライセンス]** の **[編集]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="50b98-p102">In the **Edit a user** page that opens, select the user. In the user properties page that opens, click **Edit** for **Product licenses**.</span></span>
    
3. <span data-ttu-id="50b98-p103">表示された **[製品のライセンス]** ページで、該当する **[場所]** の値を設定して、Exchange Online を含むライセンスを割り当てます (ライセンスを展開してその詳細を表示します)。完了したら、**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="50b98-p103">In the **Product licenses** page that opens, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details). When you're finished, click **Save**.</span></span>
    


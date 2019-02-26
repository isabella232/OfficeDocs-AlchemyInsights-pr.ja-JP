---
title: 126 OWA で「メールボックスが見つかりませんでした」というエラーが表示される場合
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 4/9/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: b7d54e9fb29bf94ec540e6059e932ec33f326495
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/22/2019
ms.locfileid: "30209814"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="d4d8a-102">Outlook on the web で「メールボックスが見つかりませんでした」というエラーが表示される場合</span><span class="sxs-lookup"><span data-stu-id="d4d8a-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="d4d8a-p101">Outlook on the web を使用しているときに、「**メールボックスが見つかりませんでした**」というエラーが表示された場合は、Outlook on the web への接続時に使用したアカウントに Exchange Online ライセンスが付与されていないため、そのアカウントにメールボックスが関連付けられていません。管理者は、次の手順に従ってアカウントにライセンスを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="d4d8a-p101">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account. Your admin can assign a license to your account by following these steps:</span></span> 
  
1. <span data-ttu-id="d4d8a-105">[Microsoft 365 管理センター](https://portal.office.com/adminportal/home#/homepage)を開いて、**[アクティブなユーザー]** で、**[ユーザーの編集]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4d8a-105">Open the [Office 365 admin center](https://portal.office.com/adminportal/home#/homepage) and under **Active users**, select **Edit a user**.</span></span>
    
2. <span data-ttu-id="d4d8a-p102">開いた **[ユーザーの編集]** ページで、ユーザーを選択します。開いた [ユーザーのプロパティ] ページで、**[製品のライセンス]** の **[編集]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d4d8a-p102">In the **Edit a user** page that opens, select the user. In the user properties page that opens, click **Edit** for **Product licenses**.</span></span>
    
3. <span data-ttu-id="d4d8a-p103">開いた **[製品のライセンス]** ページで、該当する **[場所]** の値を選択し、Exchange Online を含むライセンスを割り当てます (ライセンスを展開して、その詳細を表示します)。完了したら、**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d4d8a-p103">In the **Product licenses** page that opens, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details). When you're finished, click **Save**.</span></span>
    


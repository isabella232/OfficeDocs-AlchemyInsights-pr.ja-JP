---
title: 削除済みメールボックスを復元する
ms.author: pebaum
author: pebaum
ms.date: 9/12/2017
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 760587c0e58662283c3c1a647d1cc5fb81187545
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770743"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="d37d7-102">削除済みメールボックスを復元する</span><span class="sxs-lookup"><span data-stu-id="d37d7-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="d37d7-103">ユーザーの Exchange Online のライセンスが失われても、そのメールボックスは 30 日間保持され、ユーザーにライセンスを再割り当てするだけで復元できます。</span><span class="sxs-lookup"><span data-stu-id="d37d7-103">When the user loses its Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="d37d7-p101">*この機能は、30 日以内のみ有効です。* 管理ポータルから、</span><span class="sxs-lookup"><span data-stu-id="d37d7-p101">*This will work only within 30 days.*  In the Admin Portal, go to:</span></span> 
  
1. <span data-ttu-id="d37d7-p102">[**ユーザー**]、[**アクティブなユーザー**] の順に移動します。該当するユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="d37d7-p102">**Users** \> **Active** users. Select the user in question.</span></span> 
    
2. <span data-ttu-id="d37d7-108">[**編集**] を押して製品のライセンスを変更します。</span><span class="sxs-lookup"><span data-stu-id="d37d7-108">Press **Edit** to modify Product licenses</span></span> 
    
3. <span data-ttu-id="d37d7-109">Exchange Online のライセンスを割り当てて、[**保存**] を押します。</span><span class="sxs-lookup"><span data-stu-id="d37d7-109">Assign the Exchange Online license and press **Save**</span></span>
    
<span data-ttu-id="d37d7-p103">共有メールボックスを復元しようとしている場合も、復元可能な期間は 30 日間です。これらは [**ユーザー**]、[**削除済みのユーザー**] にあります。共有メールボックスにはライセンスが必要ありません。削除済みのユーザーを復元する必要が生じた場合、「[Office 365 でユーザーを復元する](https://docs.microsoft.com/office365/admin/add-users/restore-user)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d37d7-p103">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days. You can find them under **Users** \> **Deleted** users; shared mailboxes do not require a license. If you realize that you need to restore a deleted user, please see [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  


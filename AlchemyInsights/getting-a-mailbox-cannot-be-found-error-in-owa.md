---
title: 126 OWA で「メールボックスが見つかりませんでした」というエラーが表示される場合
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706755"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="275f8-102">Outlook on the web で「メールボックスが見つかりませんでした」というエラーが表示される場合</span><span class="sxs-lookup"><span data-stu-id="275f8-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="275f8-p101">Outlook on the web を使用しているときに、「**メールボックスが見つかりませんでした**」というエラーが表示された場合は、Outlook on the web への接続時に使用したアカウントに Exchange Online ライセンスが付与されていないため、そのアカウントにメールボックスが関連付けられていません。管理者は、次の手順に従ってアカウントにライセンスを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="275f8-p101">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account. Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="275f8-105">[Microsoft 365 管理センター](https://portal.office.com/adminportal/home#/homepage)を開き、[**ユーザー**] セクションの [**アクティブ ユーザー**] に移動して、エラーが表示されているユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="275f8-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="275f8-106">開いたユーザー ページで、[**ライセンスとアプリ**] セクションに移動し、該当する [**場所**] の値を選択し、Exchange Online を含むライセンスを割り当てます (ライセンスを展開して、その詳細を表示します)。</span><span class="sxs-lookup"><span data-stu-id="275f8-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="275f8-107">完了したら、[**変更の保存**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="275f8-107">When you're finished, click **Save changes**.</span></span>

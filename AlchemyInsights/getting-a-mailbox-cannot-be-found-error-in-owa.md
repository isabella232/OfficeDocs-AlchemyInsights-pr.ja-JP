---
title: 126 OWA で「メールボックスが見つかりませんでした」というエラーが表示される場合
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 4/9/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: e061ad6b74b27e3f0d597586cb2c8e31b8fa5d23
ms.sourcegitcommit: 83c644c35c2700dc515f091c8f41f9c283b89967
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/02/2020
ms.locfileid: "43105244"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="17b87-102">Outlook on the web で「メールボックスが見つかりませんでした」というエラーが表示される場合</span><span class="sxs-lookup"><span data-stu-id="17b87-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="17b87-p101">Outlook on the web を使用しているときに、「**メールボックスが見つかりませんでした**」というエラーが表示された場合は、Outlook on the web への接続時に使用したアカウントに Exchange Online ライセンスが付与されていないため、そのアカウントにメールボックスが関連付けられていません。管理者は、次の手順に従ってアカウントにライセンスを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="17b87-p101">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account. Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="17b87-105">[Microsoft 365 管理センター](https://portal.office.com/adminportal/home#/homepage)を開き、[**ユーザー**] セクションの [**アクティブ ユーザー**] に移動して、エラーが表示されているユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="17b87-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="17b87-106">開いたユーザー ページで、[**ライセンスとアプリ**] セクションに移動し、該当する [**場所**] の値を選択し、Exchange Online を含むライセンスを割り当てます (ライセンスを展開して、その詳細を表示します)。</span><span class="sxs-lookup"><span data-stu-id="17b87-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="17b87-107">完了したら、[**変更の保存**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="17b87-107">When you're finished, click **Save changes**.</span></span>

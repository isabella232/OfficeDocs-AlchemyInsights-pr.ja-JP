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
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426667"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="478a0-102">Outlook on the web で「メールボックスが見つかりませんでした」というエラーが表示される場合</span><span class="sxs-lookup"><span data-stu-id="478a0-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="478a0-p101">Outlook on the web を使用しているときに、「**メールボックスが見つかりませんでした**」というエラーが表示された場合は、Outlook on the web への接続時に使用したアカウントに Exchange Online ライセンスが付与されていないため、そのアカウントにメールボックスが関連付けられていません。管理者は、次の手順に従ってアカウントにライセンスを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="478a0-p101">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account. Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="478a0-105">[Microsoft 365 管理センター](https://portal.office.com/adminportal/home#/homepage)を開き、[**ユーザー**] セクションの [**アクティブ ユーザー**] に移動して、エラーが表示されているユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="478a0-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="478a0-106">開いたユーザー ページで、[**ライセンスとアプリ**] セクションに移動し、該当する [**場所**] の値を選択し、Exchange Online を含むライセンスを割り当てます (ライセンスを展開して、その詳細を表示します)。</span><span class="sxs-lookup"><span data-stu-id="478a0-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="478a0-107">完了したら、[**変更の保存**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="478a0-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="478a0-108">ライセンスが既にユーザー アカウントに割り当てられている場合には、ライセンスを削除して再割り当てすると、問題を解決してシステムで適切にプロビジョニングすることができます。</span><span class="sxs-lookup"><span data-stu-id="478a0-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="478a0-109">M365 Exchange Online (他の場合も) サブスクリプションが最新であり、最近期限が切れていないか確認します。</span><span class="sxs-lookup"><span data-stu-id="478a0-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="478a0-110">サブスクリプションの有効期限が切れておらず、有効なライセンスがユーザー アカウントに割り当てられている場合、ライセンスがプロビジョニングされるのに最大 24 時間かかることがあります。問題解決まで待つ必要がある場合もあります。</span><span class="sxs-lookup"><span data-stu-id="478a0-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="478a0-111">詳細については、[ライセンスの割り当てと管理](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="478a0-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>
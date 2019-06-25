---
title: "\"アクセスが拒否されました\" メッセージのトラブルシューティング"
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: a8eb435e9e19d1c5bcdb694b899e09a4126b8697
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35174506"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="d97cd-102">"アクセスが拒否されました" メッセージのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="d97cd-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="d97cd-103">Sharepoint Online サイトを参照しようとしたときにアクセス拒否メッセージを受け取った場合は、以下の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d97cd-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

<span data-ttu-id="d97cd-104">**ユーザーを追加してライセンスを付与する**</span><span class="sxs-lookup"><span data-stu-id="d97cd-104">**Add and License the user**</span></span>

<span data-ttu-id="d97cd-105">[Office 365 for business のユーザーにライセンスを割り当てる](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)ようにしてください。</span><span class="sxs-lookup"><span data-stu-id="d97cd-105">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>

<span data-ttu-id="d97cd-106">**アクセス許可の割り当て**</span><span class="sxs-lookup"><span data-stu-id="d97cd-106">**Assign Permissions**</span></span>

<span data-ttu-id="d97cd-107">ユーザーに Sharepoint ライセンスが割り当てられていて、アクセス拒否メッセージが依然として受信されている場合は、それらのユーザーに[適切なアクセス許可レベルが割り当てら](https://docs.microsoft.com/sharepoint/understanding-permission-levels)れていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="d97cd-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="d97cd-108">**アクセス要求機能の使用を検討する**</span><span class="sxs-lookup"><span data-stu-id="d97cd-108">**Consider using the access request feature**</span></span>

<span data-ttu-id="d97cd-109">[アクセス要求](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)機能を使用すると、ユーザーが現在表示する権限を持っていないコンテンツへのアクセス権を要求できます。</span><span class="sxs-lookup"><span data-stu-id="d97cd-109">The [access request](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="d97cd-110">**カスタムスクリプトを許可すると、アクセス拒否の問題が発生することがある**</span><span class="sxs-lookup"><span data-stu-id="d97cd-110">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="d97cd-111">「カスタムスクリプトを許可する」機能がアクセス拒否を提示している可能性があるシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="d97cd-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="d97cd-112">影響を受ける機能の一覧については、セキュリティに関する考慮事項と、この機能を無効にする機能を示します。</span><span class="sxs-lookup"><span data-stu-id="d97cd-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="d97cd-113">カスタムスクリプトを参照、[許可、または禁止](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)してください</span><span class="sxs-lookup"><span data-stu-id="d97cd-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="d97cd-114">注: 以前にアクセスしたことがある複数のユーザーが OneDrive または SharePoint サイトを使用できない場合は、一時的なサービスの問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d97cd-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="d97cd-115">[サービス正常性ダッシュボードをチェックし](https://portal.office.com/adminportal/home#/servicehealth)ます。</span><span class="sxs-lookup"><span data-stu-id="d97cd-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  


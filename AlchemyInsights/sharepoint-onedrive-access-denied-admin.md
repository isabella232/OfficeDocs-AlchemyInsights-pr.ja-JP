---
title: "\"アクセスが拒否されました\" メッセージのトラブルシューティング"
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751281"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="63ea5-102">Sharepoint/OneDrive 管理センターでのアクセス拒否メッセージのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="63ea5-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="63ea5-103">Sharepoint/OneDrive 管理センターを参照しようとしたときにアクセス拒否メッセージを受信した場合は、[ユーザーにライセンスを割り当てる](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)必要があります。</span><span class="sxs-lookup"><span data-stu-id="63ea5-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="63ea5-104">ユーザーがライセンスを持っている場合は、管理センターにアクセスできる[管理者の役割が割り当てら](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)れていることも確認してください。</span><span class="sxs-lookup"><span data-stu-id="63ea5-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="63ea5-105">この問題は、ユーザーを削除して、同じユーザープリンシパル名 (UPN) を使用して再作成した場合にも発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="63ea5-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="63ea5-106">新しいアカウントは、異なる PUID (Passport の一意の ID) 値を使用して作成されます。</span><span class="sxs-lookup"><span data-stu-id="63ea5-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="63ea5-107">ユーザーがサイトコレクションまたは OneDrive にアクセスしようとすると、ユーザーの誤った PUID が表示されます。</span><span class="sxs-lookup"><span data-stu-id="63ea5-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="63ea5-108">2番目のシナリオでは、Active Directory の組織単位 (OU) とのディレクトリ同期が必要になります。</span><span class="sxs-lookup"><span data-stu-id="63ea5-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="63ea5-109">ユーザーが既に SharePoint にサインインしていて、別の OU に移動して SharePoint と resynced した場合、この問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="63ea5-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="63ea5-110">この問題を解決するには、記事「 [Office 365 でユーザーを復元](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)する」の手順に従って元の UPN を復元する必要があります。</span><span class="sxs-lookup"><span data-stu-id="63ea5-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="63ea5-111">注: 以前にアクセスしたことがある複数のユーザーが OneDrive または SharePoint 管理センターを使用できない場合は、一時的なサービスの問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="63ea5-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="63ea5-112">[サービス正常性ダッシュボードをチェックし](https://portal.office.com/adminportal/home#/servicehealth)ます。</span><span class="sxs-lookup"><span data-stu-id="63ea5-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>



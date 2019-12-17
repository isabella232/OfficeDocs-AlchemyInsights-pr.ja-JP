---
title: "\"アクセスが拒否されました\" メッセージのトラブルシューティング"
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051430"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="732fb-102">Sharepoint/OneDrive 管理センターで "アクセスが拒否されました" メッセージをトラブルシューティングする</span><span class="sxs-lookup"><span data-stu-id="732fb-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="732fb-103">Sharepoint/OneDrive 管理センターをブラウザーで参照しようとしたときに、アクセス拒否のメッセージが表示された場合は、[ユーザーへのライセンス割り当て](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="732fb-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="732fb-104">ユーザーにライセンスが付与されている場合は、そのユーザーに管理センターへのアクセスを許可する[管理者の役割が割り当てられている](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)ことも確認してください。</span><span class="sxs-lookup"><span data-stu-id="732fb-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="732fb-105">この問題は、ユーザーの削除後に同じユーザー プリンシパル名 (UPN) でユーザーを再作成した場合にも発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="732fb-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="732fb-106">新しいアカウントは、別の PUID (Passport 一意識別子) を使用して作成されます。</span><span class="sxs-lookup"><span data-stu-id="732fb-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="732fb-107">そのユーザーがサイト コレクションや自分の OneDrive にアクセスしようとしたときに、ユーザーの PUID は間違ったものになります。</span><span class="sxs-lookup"><span data-stu-id="732fb-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="732fb-108">もう 1 つのシナリオには、Active Directory 組織単位 (OU) とのディレクトリ同期が関連します。</span><span class="sxs-lookup"><span data-stu-id="732fb-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="732fb-109">SharePoint にサインインしているユーザーが、別の OU に移動されて SharePoint と再同期されると、この問題が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="732fb-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="732fb-110">この問題を解決するには、「[Office 365 でユーザーを復元する](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)」に記載された手順を実行して元の UPN を復元する必要があります。</span><span class="sxs-lookup"><span data-stu-id="732fb-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="732fb-111">注: それまでアクセスできていた複数のユーザーが OneDrive または SharePoint 管理センターを利用できない場合は、サービスに一時的な問題が発生している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="732fb-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="732fb-112">[サービス正常性ダッシュボードを確認](https://portal.office.com/adminportal/home#/servicehealth)してください。</span><span class="sxs-lookup"><span data-stu-id="732fb-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>



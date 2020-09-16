---
title: "\"アクセスが拒否されました\" メッセージのトラブルシューティング"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767667"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="a4acb-102">Sharepoint/OneDrive 管理センターで "アクセスが拒否されました" メッセージをトラブルシューティングする</span><span class="sxs-lookup"><span data-stu-id="a4acb-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="a4acb-103">Sharepoint/OneDrive 管理センターをブラウザーで参照しようとしたときに、アクセス拒否のメッセージが表示された場合は、[ユーザーへのライセンス割り当て](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="a4acb-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="a4acb-104">ユーザーにライセンスが付与されている場合は、そのユーザーに管理センターへのアクセスを許可する[管理者の役割が割り当てられている](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles)ことも確認してください。</span><span class="sxs-lookup"><span data-stu-id="a4acb-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="a4acb-105">この問題は、ユーザーの削除後に同じユーザー プリンシパル名 (UPN) でユーザーを再作成した場合にも発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="a4acb-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="a4acb-106">新しいアカウントは、別の PUID (Passport 一意識別子) を使用して作成されます。</span><span class="sxs-lookup"><span data-stu-id="a4acb-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="a4acb-107">そのユーザーがサイト コレクションや自分の OneDrive にアクセスしようとしたときに、ユーザーの PUID は間違ったものになります。</span><span class="sxs-lookup"><span data-stu-id="a4acb-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="a4acb-108">もう 1 つのシナリオには、Active Directory 組織単位 (OU) とのディレクトリ同期が関連します。</span><span class="sxs-lookup"><span data-stu-id="a4acb-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="a4acb-109">SharePoint にサインインしているユーザーが、別の OU に移動されて SharePoint と再同期されると、この問題が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="a4acb-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="a4acb-110">この問題を解決するには、「[Microsoft 365 でユーザーを復元する](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)」に記載されている手順を実行して元の UPN を復元する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4acb-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="a4acb-111">注: それまでアクセスできていた複数のユーザーが OneDrive または SharePoint 管理センターを利用できない場合は、サービスに一時的な問題が発生している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a4acb-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="a4acb-112">[サービス正常性ダッシュボードを確認](https://portal.office.com/adminportal/home#/servicehealth)してください。</span><span class="sxs-lookup"><span data-stu-id="a4acb-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>



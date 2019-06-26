---
title: パフォーマンスの問題 - SharePoint または OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 9bb18196f38de473e4ee79d77bd43561ad9742e0
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223285"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="30f08-102">SharePoint または OneDrive において、処理が遅い、アクセスできない、または複数のユーザーで使用できない</span><span class="sxs-lookup"><span data-stu-id="30f08-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="30f08-103">以前にアクセスしたことがある複数のユーザーが OneDrive または SharePoint サイトを使用できない場合は、一時的なサービスの問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="30f08-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="30f08-104">[サービス正常性ダッシュボードをチェックし](https://portal.office.com/adminportal/home#/servicehealth)ます。</span><span class="sxs-lookup"><span data-stu-id="30f08-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="30f08-105">**ユーザーを追加してライセンスを付与する**</span><span class="sxs-lookup"><span data-stu-id="30f08-105">**Add and license the user**</span></span>

<span data-ttu-id="30f08-106">[Office 365 for business のユーザーにライセンスを割り当てる](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)ようにしてください。</span><span class="sxs-lookup"><span data-stu-id="30f08-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="30f08-107">**アクセス許可の割り当て**</span><span class="sxs-lookup"><span data-stu-id="30f08-107">**Assign Permissions**</span></span>

<span data-ttu-id="30f08-108">ユーザーに Sharepoint ライセンスが割り当てられていて、アクセス拒否メッセージが依然として受信されている場合は、それらのユーザーに[適切なアクセス許可レベル](https://docs.microsoft.com/sharepoint/understanding-permission-levels)が割り当てられていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="30f08-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="30f08-109">**アクセス要求機能の使用を検討する**</span><span class="sxs-lookup"><span data-stu-id="30f08-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="30f08-110">[アクセス要求機能](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)を使用すると、ユーザーが現在表示する権限を持っていないコンテンツへのアクセス権を要求できます。</span><span class="sxs-lookup"><span data-stu-id="30f08-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="30f08-111">**カスタムスクリプトを許可すると、アクセス拒否の問題が発生することがある**</span><span class="sxs-lookup"><span data-stu-id="30f08-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="30f08-112">特定のシナリオでは、[*カスタムスクリプトを許可*する] 機能がアクセス拒否を提示している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="30f08-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="30f08-113">影響を受ける機能の一覧については、セキュリティに関する考慮事項と、この機能を無効にする機能を示します。</span><span class="sxs-lookup"><span data-stu-id="30f08-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="30f08-114">[[ユーザー設定スクリプトの許可または禁止](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)] を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30f08-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


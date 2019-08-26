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
ms.openlocfilehash: 880b2bdd7b74f4365bcbff73a709d42e72be0e3a
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36535180"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="dfdf7-102">SharePoint または OneDrive において、処理が遅い、アクセスできない、または複数のユーザーで使用できない</span><span class="sxs-lookup"><span data-stu-id="dfdf7-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="dfdf7-103">それまでアクセスできていた複数のユーザーが OneDrive または SharePoint のサイトを利用できない場合は、サービスに一時的な問題が発生している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="dfdf7-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue. Check the service health dashboard</span></span> <span data-ttu-id="dfdf7-104">[サービス正常性ダッシュボードを確認](https://portal.office.com/adminportal/home#/servicehealth)してください。</span><span class="sxs-lookup"><span data-stu-id="dfdf7-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="dfdf7-105">**ユーザーの追加とライセンス認証**</span><span class="sxs-lookup"><span data-stu-id="dfdf7-105">**Add and license the user**</span></span>

<span data-ttu-id="dfdf7-106">[一般法人向け Office 365 のユーザーにライセンスが割り当てられている](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)ことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="dfdf7-106">[Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)</span></span>


<span data-ttu-id="dfdf7-107">**アクセス許可の割り当て**</span><span class="sxs-lookup"><span data-stu-id="dfdf7-107">**Assign permissions**</span></span>

<span data-ttu-id="dfdf7-108">ユーザーに SharePoint ライセンスが割り当てられていてもアクセス拒否メッセージが表示される場合は、そのユーザーに[適切なアクセス許可レベルが割り当てられている](https://docs.microsoft.com/sharepoint/understanding-permission-levels)ことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="dfdf7-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="dfdf7-109">**アクセス要求機能の使用を検討する**</span><span class="sxs-lookup"><span data-stu-id="dfdf7-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="dfdf7-110">[アクセス要求機能](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)は、ユーザーが表示する権限がないコンテンツへのアクセスを要求できるようにする機能です。</span><span class="sxs-lookup"><span data-stu-id="dfdf7-110">The access request feature allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="dfdf7-111">**カスタム スクリプトを許可するとアクセス拒否の問題が発生する可能性がある**</span><span class="sxs-lookup"><span data-stu-id="dfdf7-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="dfdf7-112">特定のシナリオでは、*カスタム スクリプトを許可*する機能を使用するとアクセス拒否が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="dfdf7-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="dfdf7-113">影響を受ける機能のリスト、セキュリティに関する考慮事項、この機能を無効にする方法については、</span><span class="sxs-lookup"><span data-stu-id="dfdf7-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="dfdf7-114">「[カスタム スクリプトを許可または禁止する](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dfdf7-114">[Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span></span>


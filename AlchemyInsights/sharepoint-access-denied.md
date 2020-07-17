---
title: "\"アクセスが拒否されました\" メッセージのトラブルシューティング"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 183f54be3230a67bfe89151a6941692de470a3e1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510505"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="163e7-102">"アクセスが拒否されました" メッセージのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="163e7-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="163e7-103">SharePoint Online のサイトを閲覧しようとしたときにアクセス拒否のメッセージが表示された場合は、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="163e7-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

<span data-ttu-id="163e7-104">**ユーザーの追加とライセンス認証**</span><span class="sxs-lookup"><span data-stu-id="163e7-104">**Add and License the user**</span></span>

<span data-ttu-id="163e7-105">[一般法人向け Microsoft 365 のユーザーにライセンスが割り当てられている](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)ことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="163e7-105">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>

<span data-ttu-id="163e7-106">**アクセス許可の割り当て**</span><span class="sxs-lookup"><span data-stu-id="163e7-106">**Assign Permissions**</span></span>

<span data-ttu-id="163e7-107">ユーザーに SharePoint ライセンスが割り当てられていてもアクセス拒否メッセージが表示される場合は、そのユーザーに[適切なアクセス許可レベルが割り当てられている](https://docs.microsoft.com/sharepoint/understanding-permission-levels)ことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="163e7-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="163e7-108">**アクセス要求機能の使用を検討する**</span><span class="sxs-lookup"><span data-stu-id="163e7-108">**Consider using the access request feature**</span></span>

<span data-ttu-id="163e7-109">[アクセス要求](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)機能は、ユーザーが表示する権限がないコンテンツへのアクセスを要求できるようにする機能です。</span><span class="sxs-lookup"><span data-stu-id="163e7-109">The [access request](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="163e7-110">**カスタム スクリプトの許可がアクセス拒否の問題の原因になることがある**</span><span class="sxs-lookup"><span data-stu-id="163e7-110">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="163e7-111">特定のシナリオでは、「カスタム スクリプトの許可」機能がアクセス拒否の発生原因になります。</span><span class="sxs-lookup"><span data-stu-id="163e7-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="163e7-112">影響を受ける機能のリストについては、セキュリティに関する考慮事項と、この機能を無効にする方法に記載されてています。</span><span class="sxs-lookup"><span data-stu-id="163e7-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="163e7-113">「[カスタム スクリプトを許可または禁止する](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="163e7-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="163e7-114">注: それまでアクセスできていた複数のユーザーが OneDrive または SharePoint のサイトを利用できない場合は、サービスに一時的な問題が発生している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="163e7-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="163e7-115">[サービス正常性ダッシュボードを確認](https://portal.office.com/adminportal/home#/servicehealth)してください。</span><span class="sxs-lookup"><span data-stu-id="163e7-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  


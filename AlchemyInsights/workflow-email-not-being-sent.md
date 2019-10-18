---
title: ワークフロー メールが送信されない
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530884"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="831b9-102">SharePoint リストまたはライブラリのワークフロー メールが送信されない</span><span class="sxs-lookup"><span data-stu-id="831b9-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="831b9-103">ワークフローからのメールがすべてのユーザーまたは特定のユーザーにのみ送信されない、または "**電子メールを送信できません。電子メールの宛先が正しいか確認してください。**" というエラーが表示される場合。</span><span class="sxs-lookup"><span data-stu-id="831b9-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="831b9-104">ユーザーがそのサイトコレクションの [**すべてのユーザー**] アクセス許可グループ (ユーザー情報リスト) に存在するかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="831b9-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="831b9-105">直接 URL のサンプル: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span><span class="sxs-lookup"><span data-stu-id="831b9-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="831b9-106">ユーザーが存在しない場合は、ユーザーがページにサインインしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="831b9-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="831b9-107">外部ユーザーの場合は、招待が承諾されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="831b9-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="831b9-108">ユーザーがアクセス許可グループに存在する場合は、メール アドレスが正しいことを確認します。</span><span class="sxs-lookup"><span data-stu-id="831b9-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="831b9-109">ユーザーのメール アドレスがアクセス許可グループで設定されていない場合は、そのユーザー用にサンプル アラートを作成します。これにより、ユーザー アカウントは SharePoint のユーザー プロファイルからこのサイト コレクションに強制的に同期されます。</span><span class="sxs-lookup"><span data-stu-id="831b9-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="831b9-110">ワークフローからのメールは、サイト コレクション管理者に送信されます。他のユーザーに送信されることはなく、**HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail** エラーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="831b9-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="831b9-111">詳細については、「[SharePoint グループに電子メールを送信するとアクセスが拒否される](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="831b9-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="831b9-112">また、サイト コレクションの機能である**制限付きアクセス ユーザーのアクセス許可ロックダウン モード**がアクティブになっていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="831b9-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="831b9-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="831b9-113">Related topics</span></span>
<span data-ttu-id="831b9-114">SharePoint Online で Microsoft Flow を試す方法。</span><span class="sxs-lookup"><span data-stu-id="831b9-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="831b9-115">フローを作成する</span><span class="sxs-lookup"><span data-stu-id="831b9-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="831b9-116">SharePoint and Flow (SharePoint と Flow)</span><span class="sxs-lookup"><span data-stu-id="831b9-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



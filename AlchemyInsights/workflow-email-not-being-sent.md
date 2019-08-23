---
title: ワークフロー電子メールが送信されていません
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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530884"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="fd580-102">ワークフロー電子メールが SharePoint リストまたはライブラリに送信されていません</span><span class="sxs-lookup"><span data-stu-id="fd580-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="fd580-103">ワークフローからの電子メールは、すべてのユーザーまたは特定のユーザーのみに送信されることはありません。また、電子メールメッセージを送信できないというエラーが表示され**ます。電子メールの受信者が有効であることを確認**します。</span><span class="sxs-lookup"><span data-stu-id="fd580-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="fd580-104">そのサイトコレクションの [**すべて**のユーザー] アクセス許可グループ (ユーザー情報リスト) にユーザーが存在するかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="fd580-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="fd580-105">サンプルの直接 URL:<tenant>https://sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?メンバーシップ Groupid = 0</span><span class="sxs-lookup"><span data-stu-id="fd580-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="fd580-106">ユーザーが存在しない場合は、ユーザーがページにサインインしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="fd580-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="fd580-107">外部ユーザーの場合は、招待状が承諾されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="fd580-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="fd580-108">ユーザーがアクセス許可グループに存在する場合は、電子メールアドレスが正しいことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="fd580-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="fd580-109">ユーザーの電子メールアドレスがここで設定されていない場合は、そのユーザーのためのサンプル通知を作成します。これにより、そのユーザーアカウントを SharePoint のユーザープロファイルからこのサイトコレクションに強制的に同期させることができます。</span><span class="sxs-lookup"><span data-stu-id="fd580-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="fd580-110">ワークフローからの電子メールは、サイトコレクションの管理者に送信されますが、他のユーザーに送信されることはありません。エラーは、 \*\* <span>https が Https</span>で禁止\*\*されています://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail。</span><span class="sxs-lookup"><span data-stu-id="fd580-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="fd580-111">[SharePoint グループに電子メールを送信する場合](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)は、「アクセス拒否」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd580-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="fd580-112">また、 **"制限付きアクセス" ユーザーアクセス許可のロックダウンモード**サイトコレクション機能がアクティブではないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="fd580-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="fd580-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="fd580-113">Related topics</span></span>
<span data-ttu-id="fd580-114">SharePoint Online で Microsoft Flow を試す場合</span><span class="sxs-lookup"><span data-stu-id="fd580-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="fd580-115">フローを作成する</span><span class="sxs-lookup"><span data-stu-id="fd580-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="fd580-116">SharePoint およびフロー</span><span class="sxs-lookup"><span data-stu-id="fd580-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



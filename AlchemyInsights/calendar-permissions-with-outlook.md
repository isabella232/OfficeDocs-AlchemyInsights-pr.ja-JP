---
title: 予定表のアクセス許可
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748798"
---
# <a name="calendar-permissions"></a><span data-ttu-id="63916-102">予定表のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="63916-102">Calendar Permissions</span></span>

<span data-ttu-id="63916-103">ユーザーは Outlook on Web やその他のクライアントで自分の予定表のアクセス許可を変更することができますが、管理者として調査を行う必要がある場合もあります。</span><span class="sxs-lookup"><span data-stu-id="63916-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="63916-104">Exchange PowerShell コマンドレットを使用すると、ユーザーの予定表のアクセス許可が表示されます。</span><span class="sxs-lookup"><span data-stu-id="63916-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="63916-105">詳細については、次のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="63916-105">To see more information see the following:</span></span>

- [<span data-ttu-id="63916-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="63916-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="63916-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="63916-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="63916-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="63916-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="63916-109">予定表のアクセス許可は、予定表の共有で使用されます。Outlook カレンダーの共有に関する詳細情報については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63916-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="63916-110">他のユーザーと Outlook 予定表を共有する</span><span class="sxs-lookup"><span data-stu-id="63916-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="63916-111">Outlook on the web の自分の予定表を仕事のために共有する</span><span class="sxs-lookup"><span data-stu-id="63916-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="63916-112">予定表のアクセス許可のトラブルシューティングを行うには、[サポート/回復アシスタント](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) ツールを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="63916-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>
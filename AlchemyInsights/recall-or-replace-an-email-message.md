---
title: 送信したメール メッセージを取り消す、または置き換えます
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: d5952041f6f2fd736e975abf06cc22880d21a089
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553437"
---
# <a name="recall-or-replace-an-email-message-in-office-365"></a><span data-ttu-id="a7ba2-102">Office 365 で電子メールメッセージを再呼び出しまたは置換する</span><span class="sxs-lookup"><span data-stu-id="a7ba2-102">Recall or replace an email message in Office 365</span></span>

- <span data-ttu-id="a7ba2-103">あなたは**あなたの組織内の人々に送られたメッセージだけを取り消すことができます**。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="a7ba2-104">たとえば、Gmail アドレスに送信された場合は、メッセージを取り消すことはできません。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-104">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="a7ba2-105">**PC の Outlook 2016 から送信されたメッセージのみを取り消す**ことができます。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-105">You can **only recall messages sent from Outlook 2016 for the PC**.</span></span> <span data-ttu-id="a7ba2-106">ユーザーが、Outlook for Mac またはOutlook on the web を使用してメッセージを送信する場合、取り消すことができません。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="a7ba2-107">管理者である場合は、 **PowerShell を使用して、ユーザーの代わりにメッセージを呼び戻す**ことができます。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-107">If you're an admin, you can **recall messages on behalf of users by using PowerShell**.</span></span> <span data-ttu-id="a7ba2-108">管理センターからメッセージを取り消すことはできません。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="a7ba2-109">詳細については、「組織内の電子メールメッセージの検索と削除」の下にスクロールしてください。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="a7ba2-110">**送信した電子メールメッセージを呼び戻すまたは置換する**</span><span class="sxs-lookup"><span data-stu-id="a7ba2-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="a7ba2-111">Outlook ウィンドウの左側にあるフォルダーウィンドウで、[送信済みアイテム] フォルダーを選択します。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="a7ba2-112">取り消したいメッセージを開きます。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-112">Open the message that you want to recall.</span></span> <span data-ttu-id="a7ba2-113">メッセージを開くには、ダブルクリックする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-113">You must double-click to open the message.</span></span> <span data-ttu-id="a7ba2-114">閲覧ウィンドウに表示されるようにメッセージを選択しても、メッセージを取り消すことはできません。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="a7ba2-115">[メッセージ] タブで、[**アクション** > を**取り消す**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="a7ba2-116">[**このメッセージの未開封のコピーを削除**する] または [**未開封のコピーを削除して新しいメッセージに置き換える**] を選択し、[ **OK]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="a7ba2-117">代替メッセージを送信している場合は、メッセージを作成し、[**送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-117">If you’re sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="a7ba2-118">メッセージの取り消しの成功または失敗は、Outlook の受信者の設定によって異なります。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="a7ba2-119">取り消しの確認方法など、詳細については、「[送信した電子メールメッセージを呼び戻すか置き換える](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="a7ba2-120">***組織内の電子メールメッセージの検索と削除***組織内の電子メールメッセージを検索して削除するには、グローバル管理者であることが最も簡単です。グローバル管理者でない場合は、アカウントが電子情報開示マネージャーの役割グループまたはコンプライアンス検索管理役割に追加されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-120">***Search for and delete email messages in your organization*** To search for and delete email messages in your organization, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="a7ba2-121">メッセージを削除するには、Organization Management ロールグループのメンバーであるか、検索と消去の管理ロールが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="a7ba2-122">これらの役割へのアクセス許可は、[セキュリティ & コンプライアンスセンター](https://protection.office.com/)で割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="a7ba2-123">[コンテンツ検索を作成し、](https://docs.microsoft.com/office365/securitycompliance/content-search) 削除するメッセージを見つけます。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-123">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="a7ba2-124">[セキュリティ & コンプライアンスセンター PowerShell に接続](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)します。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span> 

<span data-ttu-id="a7ba2-125">MFA を使用している場合は、「 [Connect To Office 365 Security & 多要素認証を使用](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)した PowerShell」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7ba2-125">If you're using MFA, see [Connect to Office 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span> 

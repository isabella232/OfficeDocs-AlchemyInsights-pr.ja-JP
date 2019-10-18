---
title: メール メッセージを取り消す、または置き換える
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553437"
---
# <a name="recall-or-replace-an-email-message-in-office-365"></a><span data-ttu-id="875c6-102">Office 365 でメール メッセージを取り消す、または置き換える</span><span class="sxs-lookup"><span data-stu-id="875c6-102">Recall or replace an email message in Office 365</span></span>

- <span data-ttu-id="875c6-103">あなたは**あなたの組織内の人々に送られたメッセージだけを取り消すことができます**。</span><span class="sxs-lookup"><span data-stu-id="875c6-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="875c6-104">たとえば、Gmail アドレスに送信された場合は、メッセージを取り消すことはできません。</span><span class="sxs-lookup"><span data-stu-id="875c6-104">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="875c6-105">**PC 版 Outlook 2016 から送信されたメッセージだけを取り消すことができます**。</span><span class="sxs-lookup"><span data-stu-id="875c6-105">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="875c6-106">ユーザーが、Outlook for Mac またはOutlook on the web を使用してメッセージを送信する場合、取り消すことができません。</span><span class="sxs-lookup"><span data-stu-id="875c6-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="875c6-107">管理者であれば、**PowerShell を使用してユーザーの代理のメッセージを取り消すことが**できます。</span><span class="sxs-lookup"><span data-stu-id="875c6-107">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="875c6-108">管理センターからメッセージを取り消すことはできません。</span><span class="sxs-lookup"><span data-stu-id="875c6-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="875c6-109">下にスクロールして、「Office 365 組織でメール メッセージの検索と削除を行う」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="875c6-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="875c6-110">**送信したメール メッセージを取り消す、または置き換える**</span><span class="sxs-lookup"><span data-stu-id="875c6-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="875c6-111">Outlook ウィンドウの左側のフォルダー ペインで、[送信済みアイテム] フォルダーを選びます。</span><span class="sxs-lookup"><span data-stu-id="875c6-111">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
2. <span data-ttu-id="875c6-112">取り消すメッセージを開きます。</span><span class="sxs-lookup"><span data-stu-id="875c6-112">Open the message that contains the attachment you want to print.</span></span> <span data-ttu-id="875c6-113">メッセージを開くにはダブルクリックする必要があります。</span><span class="sxs-lookup"><span data-stu-id="875c6-113">You must double-click to open the message.</span></span> <span data-ttu-id="875c6-114">閲覧ウィンドウに表示されるようにメッセージを選択しても、メッセージを取り消すことはできません。</span><span class="sxs-lookup"><span data-stu-id="875c6-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="875c6-115">[メッセージ] タブから、[**操作]、[** > **メッセージの取り消し**]を選択します。</span><span class="sxs-lookup"><span data-stu-id="875c6-115">Select the Message tab, and then select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="875c6-116">[**未読のこのメッセージのコピーを削除する**]、または [**未読のコピーを削除して新しいメッセージに置き換える**] を選び、それから [**OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="875c6-116">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
5. <span data-ttu-id="875c6-117">代わりのメッセージを送信する場合、メッセージを作成し、[**送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="875c6-117">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
6. <span data-ttu-id="875c6-118">メッセージ取り消しの成功または失敗は、受信者の Outlook の設定によって決まります。</span><span class="sxs-lookup"><span data-stu-id="875c6-118">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span>

<span data-ttu-id="875c6-119">取り消しを確認する方法など、詳細については、「[送信したメールメッセージを取り消す、または置き換える](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="875c6-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="875c6-120">***組織内の電子メールメッセージを検索して削除する*** 組織内の電子メールメッセージを検索して削除するには、グローバル管理者であることが最も簡単です。グローバル管理者でない場合は、アカウントを eDiscovery Manager のロールグループ、または Compliance Search の管理ロールに追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="875c6-120">***Search for and delete email messages in your organization*** To search for and delete email messages in your organization, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="875c6-121">メッセージを削除するには、Organization Management ロールグループのメンバーであるか、検索と消去の管理ロールが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="875c6-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="875c6-122">これらのロールへの権限は、[セキュリティ/コンプライアンス センター](https://protection.office.com/)で付与されます。</span><span class="sxs-lookup"><span data-stu-id="875c6-122">Permissions for these roles are assigned in the [Security and compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="875c6-123">[コンテンツ検索を作成し、](https://docs.microsoft.com/office365/securitycompliance/content-search) 削除するメッセージを見つけます。</span><span class="sxs-lookup"><span data-stu-id="875c6-123">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="875c6-124">[セキュリティ/コンプライアンス センターの PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="875c6-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)</span></span> 

<span data-ttu-id="875c6-125">MFA をお使いの場合は、「[多要素認証を使用して Office 365 セキュリティ センター/コンプライアンス センターの PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="875c6-125">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span> 

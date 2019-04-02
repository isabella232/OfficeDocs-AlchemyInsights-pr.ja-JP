---
title: Outlook デスクトップでメール メッセージを取り消す、または置き換えます
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/15/2019
ms.locfileid: "31014858"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="e4cee-102">送信したメール メッセージを取り消す、または置き換えます</span><span class="sxs-lookup"><span data-stu-id="e4cee-102">Outlook Desktop recall or replace an email message</span></span>

- <span data-ttu-id="e4cee-103">管理者は、**PowerShell を使用してユーザーの代理のメッセージを取り消すことが**できます。</span><span class="sxs-lookup"><span data-stu-id="e4cee-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="e4cee-104">管理センターからメッセージを取り消すことはできません。</span><span class="sxs-lookup"><span data-stu-id="e4cee-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="e4cee-105">あなたは**あなたの組織内の人々に送られたメッセージだけを取り消すことができます**。</span><span class="sxs-lookup"><span data-stu-id="e4cee-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="e4cee-106">たとえば、Gmail アドレスに送信された場合は、メッセージを取り消すことはできません。</span><span class="sxs-lookup"><span data-stu-id="e4cee-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="e4cee-107">あなたは **PC の Outlook 2016 から送信されたメッセージだけを取り消すことができます**。</span><span class="sxs-lookup"><span data-stu-id="e4cee-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="e4cee-108">ユーザーが、Outlook for Mac またはOutlook on the web を使用してメッセージを送信する場合、取り消すことができません。</span><span class="sxs-lookup"><span data-stu-id="e4cee-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="e4cee-109">送信したメール メッセージを取り消す、または置き換えるには：</span><span class="sxs-lookup"><span data-stu-id="e4cee-109">Outlook Desktop recall or replace an email message</span></span>

1. <span data-ttu-id="e4cee-110">Outlook ウィンドウの左側のフォルダー ペインで、[送信済みアイテム] フォルダーを選択します。</span><span class="sxs-lookup"><span data-stu-id="e4cee-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="e4cee-111">取り消したいメッセージをクリックして開きます。</span><span class="sxs-lookup"><span data-stu-id="e4cee-111">Double-click the scorecard that you want to change to open it.</span></span>
1. <span data-ttu-id="e4cee-112">**メッセージ**タブを選択、それから**Actions** > **Recall This Message**を選択。</span><span class="sxs-lookup"><span data-stu-id="e4cee-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="e4cee-113">[**未読のこのメッセージのコピーを削除する**]を選択、または [**未読のコピーを削除して新しいメッセージに置き換える**] 、そして[**OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e4cee-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="e4cee-114">代わりのメッセージを送信する場合、メッセージを作成し、[**送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e4cee-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="e4cee-115">メッセージ取り消しの成功または失敗は、受信者のOutlookの設定によって決まります。</span><span class="sxs-lookup"><span data-stu-id="e4cee-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="e4cee-116">取り消しの状況をチェックするステップについては、[こちらの記事](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4cee-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="e4cee-117">組織内の電子メールメッセージを検索して削除します</span><span class="sxs-lookup"><span data-stu-id="e4cee-117">Search for and delete email messages in your Office 365 organization</span></span>

- <span data-ttu-id="e4cee-118">グローバル管理者ではない場合、メッセージを検索するには、自分のアカウントをeDiscovery ManagerロールまたはCompliance Search管理ロールに追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4cee-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="e4cee-119">メッセージを削除するには、Organization Management ロールグループのメンバーであるか、検索と消去の管理ロールが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4cee-119">To delete messages, you have to be a member of the Organization Management role group or be assigned the Search And Purge management role.</span></span> <span data-ttu-id="e4cee-120">これらのロールの権限は、[セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/?linkid=2083731)で付与されます。</span><span class="sxs-lookup"><span data-stu-id="e4cee-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="e4cee-121">[コンテンツ検索を作成し、](https://docs.microsoft.com/office365/securitycompliance/content-search) 削除するメッセージを見つけます。</span><span class="sxs-lookup"><span data-stu-id="e4cee-121">Step 1: Create a Content Search to find the message to delete</span></span>
- <span data-ttu-id="e4cee-122">[セキュリティ/コンプライアンス センターのPowerShellに接続します](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="e4cee-122">[Connect to the Security and Compliance Center via Remote PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)</span></span>

<span data-ttu-id="e4cee-123">多要素認証を使用している場合、以下を参照してください [多要素認証を使用してOffice 365のセキュリティ/コンプライアンス センターのPowerShellに接続する](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="e4cee-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>
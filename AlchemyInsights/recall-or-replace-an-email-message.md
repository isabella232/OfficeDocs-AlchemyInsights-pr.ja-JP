---
title: 送信したメール メッセージを取り消す、または置き換えます
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353511"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="29929-102">Microsoft 365 でメール メッセージを取り消す、または置き換える</span><span class="sxs-lookup"><span data-stu-id="29929-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="29929-103">あなたは **あなたの組織内の人々に送られたメッセージだけを取り消すことができます**。</span><span class="sxs-lookup"><span data-stu-id="29929-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="29929-104">たとえば、Gmail アドレスに送信された場合は、メッセージを取り消すことはできません。</span><span class="sxs-lookup"><span data-stu-id="29929-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="29929-105">**PC 版 Outlook から送信されたメッセージのみを取り消すことができます**。</span><span class="sxs-lookup"><span data-stu-id="29929-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="29929-106">ユーザーが、Outlook for Mac またはOutlook on the web を使用してメッセージを送信する場合、取り消すことができません。</span><span class="sxs-lookup"><span data-stu-id="29929-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="29929-107">テナント管理者は、**PowerShell を使用してユーザーに代わってメッセージを取り消す** ことができます (詳細については、「[メール メッセージの検索と削除](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)」を参照してください)。</span><span class="sxs-lookup"><span data-stu-id="29929-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="29929-108">管理センターからメッセージを取り消すことはできません。</span><span class="sxs-lookup"><span data-stu-id="29929-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="29929-109">下にスクロールして、「Office 365 組織でメール メッセージの検索と削除を行う」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29929-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="29929-110">**送信したメール メッセージを取り消す、または置き換える**</span><span class="sxs-lookup"><span data-stu-id="29929-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="29929-111">Outlook ウィンドウの左側のフォルダー ペインで、[送信済みアイテム] フォルダーを選びます。</span><span class="sxs-lookup"><span data-stu-id="29929-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="29929-112">取り消すメッセージを開きます。</span><span class="sxs-lookup"><span data-stu-id="29929-112">Open the message that you want to recall.</span></span> <span data-ttu-id="29929-113">メッセージを開くにはダブルクリックする必要があります。</span><span class="sxs-lookup"><span data-stu-id="29929-113">You must double-click to open the message.</span></span> <span data-ttu-id="29929-114">閲覧ウィンドウに表示されるようにメッセージを選択しても、メッセージを取り消すことはできません。</span><span class="sxs-lookup"><span data-stu-id="29929-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="29929-115">[メッセージ] タブから、[**操作]、[** > **メッセージの取り消し**]を選択します。</span><span class="sxs-lookup"><span data-stu-id="29929-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="29929-116">[**未読のこのメッセージのコピーを削除する**]、または [**未読のコピーを削除して新しいメッセージに置き換える**] を選び、それから [**OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="29929-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="29929-117">代わりのメッセージを送信する場合、メッセージを作成し、**[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="29929-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="29929-118">メッセージ取り消しの成功または失敗は、受信者の Outlook の設定によって決まります。</span><span class="sxs-lookup"><span data-stu-id="29929-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="29929-119">取り消しを確認する方法など、詳細については、「[送信したメールメッセージを取り消す、または置き換える](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29929-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="29929-120">**_組織内のメール メッセージを検索して削除するには_**、グローバル管理者であることが最も簡単です。グローバル管理者でない場合は、アカウントを電子情報開示マネージャーの役割グループ、またはコンプライアンス検索の管理の役割に追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="29929-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="29929-121">メッセージを削除するには、Organization Management ロールグループのメンバーであるか、検索と消去の管理ロールが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="29929-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="29929-122">これらのロールへの権限は、[セキュリティ/コンプライアンス センター](https://protection.office.com/)で付与されます。</span><span class="sxs-lookup"><span data-stu-id="29929-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="29929-123">[コンテンツ検索を作成し、](https://docs.microsoft.com/microsoft-365/compliance/content-search) 削除するメッセージを見つけます。</span><span class="sxs-lookup"><span data-stu-id="29929-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="29929-124">[セキュリティ/コンプライアンス センターの PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)。</span><span class="sxs-lookup"><span data-stu-id="29929-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="29929-125">多要素認証 (MFA) を使用している場合、「[多要素認証を使用して Microsoft 365 セキュリティ/コンプライアンス センター PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29929-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>

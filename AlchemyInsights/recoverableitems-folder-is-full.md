---
title: 1336 [回復可能なアイテム] フォルダーに空きがない
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510757"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="db462-102">[回復可能なアイテム] フォルダーに空きがない</span><span class="sxs-lookup"><span data-stu-id="db462-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="db462-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span><span class="sxs-lookup"><span data-stu-id="db462-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="db462-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span><span class="sxs-lookup"><span data-stu-id="db462-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="db462-105">[回復可能なアイテム] フォルダーが記憶域の制限に達すると、メールボックスの機能は次のように影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="db462-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="db462-106">ユーザーは、メールボックスからアイテムを削除できません。</span><span class="sxs-lookup"><span data-stu-id="db462-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="db462-107">管理フォルダー アシスタントは、保持タグや管理フォルダー設定をもとにしてアイテムを削除できません。</span><span class="sxs-lookup"><span data-stu-id="db462-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="db462-108">単一アイテムの回復が有効になっているメールボックスまたは訴訟ホールドに配置されているメールボックスでは、コピー オン ライト ページ保護プロセスが、ユーザーにより編集されたアイテムのバージョンを維持できません。</span><span class="sxs-lookup"><span data-stu-id="db462-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="db462-109">メールボックス監査ログが有効なメールボックスで、[回復可能なアイテム] フォルダーの Audits サブフォルダーにメールボックス ログ エントリを保存できません。</span><span class="sxs-lookup"><span data-stu-id="db462-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="db462-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span><span class="sxs-lookup"><span data-stu-id="db462-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="db462-111">For more information, see the following topics:</span><span class="sxs-lookup"><span data-stu-id="db462-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="db462-112">メッセージを検索して削除する</span><span class="sxs-lookup"><span data-stu-id="db462-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="db462-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="db462-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="db462-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span><span class="sxs-lookup"><span data-stu-id="db462-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="db462-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="db462-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="db462-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span><span class="sxs-lookup"><span data-stu-id="db462-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="db462-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="db462-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>

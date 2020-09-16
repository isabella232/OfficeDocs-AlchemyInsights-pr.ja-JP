---
title: 1336 [回復可能なアイテム] フォルダーに空きがない
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741272"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="5f176-102">[回復可能なアイテム] フォルダーに空きがない</span><span class="sxs-lookup"><span data-stu-id="5f176-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="5f176-p101">Exchange Online メールボックスの場合、[回復可能なアイテム] フォルダーの記憶域の既定の制限は 30 GB です。メールボックスが訴訟ホールドまたは電子情報開示の保留リストに配置されるか、アイテム保持ポリシーに割り当てられている場合、[回復可能なアイテム] フォルダーの記憶域の制限は自動的に 100 GB に増やされます。</span><span class="sxs-lookup"><span data-stu-id="5f176-p101">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="5f176-105">[回復可能なアイテム] フォルダーが記憶域の制限に達すると、メールボックスの機能は次のように影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="5f176-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="5f176-106">ユーザーは、メールボックスからアイテムを削除できません。</span><span class="sxs-lookup"><span data-stu-id="5f176-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="5f176-107">管理フォルダー アシスタントは、保持タグや管理フォルダー設定をもとにしてアイテムを削除できません。</span><span class="sxs-lookup"><span data-stu-id="5f176-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="5f176-108">単一アイテムの回復が有効になっているメールボックスまたは訴訟ホールドに配置されているメールボックスでは、コピー オン ライト ページ保護プロセスが、ユーザーにより編集されたアイテムのバージョンを維持できません。</span><span class="sxs-lookup"><span data-stu-id="5f176-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="5f176-109">メールボックス監査ログが有効なメールボックスで、[回復可能なアイテム] フォルダーの Audits サブフォルダーにメールボックス ログ エントリを保存できません。</span><span class="sxs-lookup"><span data-stu-id="5f176-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="5f176-p102">保留になっていないメールボックスの場合、管理者は Exchange Online PowerShell の `Search-Mailbox -SearchDumpsterOnly -DeleteContent` コマンドを使用して [回復可能なアイテム] フォルダー内のアイテムを削除できます。詳細については、以下のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f176-p102">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span>

- [<span data-ttu-id="5f176-112">メッセージを検索して削除する</span><span class="sxs-lookup"><span data-stu-id="5f176-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="5f176-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="5f176-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="5f176-p103">保持中のメールボックスでは、先に保留リストを削除しなければ、[回復可能なアイテム] フォルダーのアイテムを削除することはできません。詳細については、「[保留中のクラウド ベースのメールボックスの [回復可能なアイテム] フォルダーのアイテムを削除する](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5f176-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="5f176-p104">[回復可能なアイテム] フォルダーがいっぱいになるのを防ぐには、管理者は保持中のメールボックスに対する [回復可能なアイテム] フォルダーの記憶域制限を増やし、[回復可能なアイテム] フォルダーからユーザーのアーカイブ メールボックスにアイテムを移動するメールボックス保持ポリシーを設定することができます。「[保持中のメールボックスの [回復可能なアイテム] のクォータを拡大する](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5f176-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>

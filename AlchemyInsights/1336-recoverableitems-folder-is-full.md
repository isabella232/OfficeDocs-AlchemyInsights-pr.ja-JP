---
title: 1336 RecoverableItems フォルダーがいっぱい
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297554"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="b0eda-102">回復可能なアイテム フォルダーがいっぱい</span><span class="sxs-lookup"><span data-stu-id="b0eda-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="b0eda-p101">Office 365 のオンラインの Exchange メールボックスは、回復可能なアイテム] フォルダーの既定の格納域の制限は 30 GB です。メールボックスは、証拠保全、電子的証拠開示の保留リストに配置または Office 365 のリテンション ・ ポリシーに割り当てられた場合、100 GB に、回復可能なアイテム] フォルダーの格納域の制限が自動的に増加します。</span><span class="sxs-lookup"><span data-stu-id="b0eda-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="b0eda-105">回復可能な項目] フォルダーでは、格納域の制限に達すると、メールボックスの機能は次の方法で影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="b0eda-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="b0eda-106">ユーザーは、メールボックスからアイテムを削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="b0eda-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="b0eda-107">管理フォルダー アシスタントが、保持タグや管理フォルダー設定をもとにしてアイテムを削除できない。</span><span class="sxs-lookup"><span data-stu-id="b0eda-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="b0eda-108">有効になっている 1 つのアイテムの回復または保留中のメールボックスのコピー オン ライト ページ保護プロセスは、ユーザーを編集する項目のバージョンを維持できません。</span><span class="sxs-lookup"><span data-stu-id="b0eda-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="b0eda-109">監査ログを有効にするメールボックスのあるメールボックスのメールボックス監査ログ エントリできますに保存されません、回復可能なアイテム] フォルダー内のサブフォルダーに監査します。</span><span class="sxs-lookup"><span data-stu-id="b0eda-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="b0eda-p102">保留リストに登録されていないメールボックスでは、管理者が使用して、`Search-Mailbox -SearchDumpsterOnly -DeleteContent`で、回復可能なアイテム] フォルダー内のアイテムを削除するのには、Exchange オンライン PowerShell コマンドです。詳細については、次のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0eda-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="b0eda-112">メッセージを検索して削除する</span><span class="sxs-lookup"><span data-stu-id="b0eda-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="b0eda-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="b0eda-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="b0eda-p103">保留中のメールボックスの回復可能なアイテム] フォルダーから削除済みアイテムを前に、保留リストを削除するのには管理者があります。詳細については、[クラウド ベースのメールボックスのフォルダーを保持する回復可能な項目で項目の削除](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0eda-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="b0eda-p104">いっぱいになるたびに、回復可能なアイテム] フォルダーを防ぐため、管理者が上のメールボックスのフォルダーを保持し、ユーザーのアーカイブを回復可能なアイテム] フォルダーからアイテムを移動するメールボックスの保持ポリシーを設定は、回復可能な項目の格納域の制限を増やすことができます。メールボックスです。[上のメールボックスのクォータを保持する回復可能な項目の増加](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0eda-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  


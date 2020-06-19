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
# <a name="the-recoverable-items-folder-is-full"></a>[回復可能なアイテム] フォルダーに空きがない

For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.

[回復可能なアイテム] フォルダーが記憶域の制限に達すると、メールボックスの機能は次のように影響を受けます。

- ユーザーは、メールボックスからアイテムを削除できません。

- 管理フォルダー アシスタントは、保持タグや管理フォルダー設定をもとにしてアイテムを削除できません。

- 単一アイテムの回復が有効になっているメールボックスまたは訴訟ホールドに配置されているメールボックスでは、コピー オン ライト ページ保護プロセスが、ユーザーにより編集されたアイテムのバージョンを維持できません。

- メールボックス監査ログが有効なメールボックスで、[回復可能なアイテム] フォルダーの Audits サブフォルダーにメールボックス ログ エントリを保存できません。

For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:

- [メッセージを検索して削除する](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).

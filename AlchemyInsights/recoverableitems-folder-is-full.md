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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741272"
---
# <a name="the-recoverable-items-folder-is-full"></a>[回復可能なアイテム] フォルダーに空きがない

Exchange Online メールボックスの場合、[回復可能なアイテム] フォルダーの記憶域の既定の制限は 30 GB です。メールボックスが訴訟ホールドまたは電子情報開示の保留リストに配置されるか、アイテム保持ポリシーに割り当てられている場合、[回復可能なアイテム] フォルダーの記憶域の制限は自動的に 100 GB に増やされます。

[回復可能なアイテム] フォルダーが記憶域の制限に達すると、メールボックスの機能は次のように影響を受けます。

- ユーザーは、メールボックスからアイテムを削除できません。

- 管理フォルダー アシスタントは、保持タグや管理フォルダー設定をもとにしてアイテムを削除できません。

- 単一アイテムの回復が有効になっているメールボックスまたは訴訟ホールドに配置されているメールボックスでは、コピー オン ライト ページ保護プロセスが、ユーザーにより編集されたアイテムのバージョンを維持できません。

- メールボックス監査ログが有効なメールボックスで、[回復可能なアイテム] フォルダーの Audits サブフォルダーにメールボックス ログ エントリを保存できません。

保留になっていないメールボックスの場合、管理者は Exchange Online PowerShell の `Search-Mailbox -SearchDumpsterOnly -DeleteContent` コマンドを使用して [回復可能なアイテム] フォルダー内のアイテムを削除できます。詳細については、以下のトピックを参照してください。

- [メッセージを検索して削除する](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

保持中のメールボックスでは、先に保留リストを削除しなければ、[回復可能なアイテム] フォルダーのアイテムを削除することはできません。詳細については、「[保留中のクラウド ベースのメールボックスの [回復可能なアイテム] フォルダーのアイテムを削除する](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)」をご覧ください。

[回復可能なアイテム] フォルダーがいっぱいになるのを防ぐには、管理者は保持中のメールボックスに対する [回復可能なアイテム] フォルダーの記憶域制限を増やし、[回復可能なアイテム] フォルダーからユーザーのアーカイブ メールボックスにアイテムを移動するメールボックス保持ポリシーを設定することができます。「[保持中のメールボックスの [回復可能なアイテム] のクォータを拡大する](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)」をご覧ください。

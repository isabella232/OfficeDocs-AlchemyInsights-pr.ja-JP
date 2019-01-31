---
title: 1336 [回復可能なアイテム] フォルダーに空きがない
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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477024"
---
# <a name="the-recoverable-items-folder-is-full"></a>[回復可能なアイテム] フォルダーに空きがない

Office 365 の Exchange Online メールボックスの場合、[回復可能なアイテム] フォルダーの記憶域の既定の制限は 30 GB です。メールボックスが訴訟ホールドまたは電子情報開示の保留リストに配置されるか、Office 365 のアイテム保持ポリシーに割り当てられている場合、[回復可能なアイテム] フォルダーの記憶域の制限は自動的に 100 GB に増やされます。
  
[回復可能なアイテム] フォルダーが記憶域の制限に達すると、メールボックスの機能は次のように影響を受けます。
  
- ユーザーは、メールボックスからアイテムを削除できません。
    
- 管理フォルダー アシスタントは、保持タグや管理フォルダー設定をもとにしてアイテムを削除できません。
    
- 単一アイテムの回復が有効になっているメールボックスまたは訴訟ホールドに配置されているメールボックスでは、コピー オン ライト ページ保護プロセスが、ユーザーにより編集されたアイテムのバージョンを維持できません。
    
- メールボックス監査ログが有効なメールボックスで、[回復可能なアイテム] フォルダーの Audits サブフォルダーにメールボックス ログ エントリを保存できません。
    
保持中でないメールボックスでは、管理者は Exchange Online PowerShell の `Search-Mailbox -SearchDumpsterOnly -DeleteContent` コマンドを使用して、[回復可能なアイテム] フォルダーのアイテムを削除できます。詳細については、次のトピックをご覧ください。 
  
- [メッセージを検索して削除する](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
保持中のメールボックスでは、先に保留リストを削除しなければ、[回復可能なアイテム] フォルダーのアイテムを削除することはできません。詳細については、「[保留中のクラウド ベースのメールボックスの [回復可能なアイテム] フォルダーのアイテムを削除する](https://docs.microsoft.com/ja-JP/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)」をご覧ください。
  
[回復可能なアイテム] フォルダーがいっぱいになるのを防ぐには、管理者は保持中のメールボックスに対する [回復可能なアイテム] フォルダーの記憶域制限を増やし、[回復可能なアイテム] フォルダーからユーザーのアーカイブ メールボックスにアイテムを移動するメールボックス保持ポリシーを設定することができます。「[保持中のメールボックスの [回復可能なアイテム] のクォータを拡大する](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)」をご覧ください。
  


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
# <a name="the-recoverable-items-folder-is-full"></a>回復可能なアイテム フォルダーがいっぱい

Office 365 のオンラインの Exchange メールボックスは、回復可能なアイテム] フォルダーの既定の格納域の制限は 30 GB です。メールボックスは、証拠保全、電子的証拠開示の保留リストに配置または Office 365 のリテンション ・ ポリシーに割り当てられた場合、100 GB に、回復可能なアイテム] フォルダーの格納域の制限が自動的に増加します。
  
回復可能な項目] フォルダーでは、格納域の制限に達すると、メールボックスの機能は次の方法で影響を受けます。
  
- ユーザーは、メールボックスからアイテムを削除することはできません。
    
- 管理フォルダー アシスタントが、保持タグや管理フォルダー設定をもとにしてアイテムを削除できない。
    
- 有効になっている 1 つのアイテムの回復または保留中のメールボックスのコピー オン ライト ページ保護プロセスは、ユーザーを編集する項目のバージョンを維持できません。
    
- 監査ログを有効にするメールボックスのあるメールボックスのメールボックス監査ログ エントリできますに保存されません、回復可能なアイテム] フォルダー内のサブフォルダーに監査します。
    
保留リストに登録されていないメールボックスでは、管理者が使用して、`Search-Mailbox -SearchDumpsterOnly -DeleteContent`で、回復可能なアイテム] フォルダー内のアイテムを削除するのには、Exchange オンライン PowerShell コマンドです。詳細については、次のトピックを参照してください。 
  
- [メッセージを検索して削除する](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
保留中のメールボックスの回復可能なアイテム] フォルダーから削除済みアイテムを前に、保留リストを削除するのには管理者があります。詳細については、[クラウド ベースのメールボックスのフォルダーを保持する回復可能な項目で項目の削除](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)を参照してください。
  
いっぱいになるたびに、回復可能なアイテム] フォルダーを防ぐため、管理者が上のメールボックスのフォルダーを保持し、ユーザーのアーカイブを回復可能なアイテム] フォルダーからアイテムを移動するメールボックスの保持ポリシーを設定は、回復可能な項目の格納域の制限を増やすことができます。メールボックスです。[上のメールボックスのクォータを保持する回復可能な項目の増加](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)を参照してください。
  


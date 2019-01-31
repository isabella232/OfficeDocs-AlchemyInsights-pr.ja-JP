---
title: 動作していない Exchange 管理センターでの保存ポリシー
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6c69511f6bcdad5793cd2473a20a2d168d2ac260
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660712"
---
 **問題:** 新しく作成されたメールボックスに、Exchange 管理センターで最新のリテンション ・ ポリシーを適用しないまたはアイテムのアーカイブ メールボックスに移動または削除はできません。 
  
 **根本的な原因。**
  
- **管理フォルダー アシスタント**は処理されないため、ユーザーのメールボックスがあります。管理フォルダー アシスタントを 7 日間に 1 回に、クラウド ベース組織内のすべてのメールボックスの処理を試みます。保持タグを変更するメールボックスに異なるアイテム保持ポリシーを適用するか、待つことができます。、メールボックスを処理する、管理フォルダーを支援または管理フォルダー アシスタントに特定の処理を開始する開始 ManagedFolderAssistant コマンドレットを実行することができます。メールボックスです。このコマンドレットを実行することがテストまたは保持ポリシーまたは保持タグ設定のトラブルシューティングに便利です。詳細については、[管理フォルダー アシスタントの実行](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)を参照してください。
    
  - **ソリューション:** 管理フォルダー アシスタントに特定のメールボックスを開始する次のコマンドを実行します。 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- **RetentionHold**は、メールボックスで**有効になっている**がされている場合これも発生します。場合は、RetentionHold には、メールボックスが置かれた、その時に、メールボックスに保持ポリシーは処理されません。詳細については、RetentionHold の設定を参照してください:[メールボックスの保存を保持](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)します。
    
    **ソリューション:**
    
  - [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)では、特定のメールボックスに RetentionHold の設定の状態を確認します。
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - 特定のメールボックスでは、RetentionHold**を無効にするの**には、次のコマンドを実行します。 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - ここで、管理フォルダー アシスタントを再実行します。
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **注:** メールボックスが 10 MB より小さい場合は、管理フォルダー アシスタントはいない自動的にメールボックスの処理です。 
  


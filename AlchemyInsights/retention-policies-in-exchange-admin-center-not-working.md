---
title: Exchange 管理センターでアイテム保持ポリシーが動作しない
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551348"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange 管理センターでのアイテム保持ポリシー

 **問題:** Exchange 管理センターで新規作成または更新したアイテム保持ポリシーがメールボックスに適用されないか、アイテムがアーカイブ メールボックスに移動または削除されません。 
  
 **原因:**
  
- これは、**管理フォルダー用アシスタント**が、ユーザーのメールボックスを処理していないことが原因である可能性があります。管理フォルダー用アシスタントは、クラウド ベースの組織のすべてのメールボックスの処理を 7 日間に 1 回試行します。ユーザーが保持タグを変更した場合やメールボックスに別のアイテム保持ポリシーを適用した場合は、管理フォルダー アシスタントによってメールボックスが処理されるまで待つか、Start-ManagedFolderAssistant コマンドレットを実行して、管理フォルダー用アシスタントによって特定のメールボックスの処理が開始されるようにします。このコマンドレットの実行は、アイテム保持ポリシーまたは保持タグの設定をテストまたはトラブルシューティングするのに便利です。詳細については、[管理フォルダー用アシスタントの実行](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)に関するページを参照してください。
    
  - **解決方法:** 特定のメールボックスに対して管理フォルダー用アシスタントを開始するには、次のコマンドを実行します。
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- これは、メールボックスで**保持ホールド**が**有効**になっている場合にも発生する可能性があります。メールボックスが保持ホールドになっている場合、その期間、そのメールボックスに対してアイテム保持ポリシーは処理されません。保持ホールドの設定の詳細については、[メールボックスの保持ホールド](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)に関するページを参照してください。
    
    **解決方法:**
    
  - [EXO Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) を使用して、特定のメールボックスの保持ホールドの設定を確認します。
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - 特定のメールボックスの保持ホールドを**無効**にするには、次のコマンドを実行します。
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - 次に、管理フォルダー用アシスタントを再実行します。
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **注:** メールボックス サイズが 10 MB 未満の場合、管理フォルダー用アシスタントによってメールボックスは自動処理されません。
 
Exchange 管理センターのアイテム保持ポリシーの詳細については、次の情報を参照してください。
- [保持タグおよびアイテム保持ポリシー](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [メールボックスにアイテム保持ポリシーを適用する](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [アイテム保持タグの追加または削除](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [メールボックスにかけられた保留の種類を識別する方法](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)

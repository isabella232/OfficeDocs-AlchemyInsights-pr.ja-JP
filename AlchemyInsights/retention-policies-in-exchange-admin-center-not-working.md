---
title: Exchange 管理センターでアイテム保持ポリシーが動作しない
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502612"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange 管理センターでのアイテム保持ポリシー

 **問題:** Exchange 管理センターで新規作成または更新したアイテム保持ポリシーがメールボックスに適用されないか、アイテムがアーカイブ メールボックスに移動または削除されません。 
  
 **原因:**
  
- This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **解決方法:** 特定のメールボックスに対して管理フォルダー用アシスタントを開始するには、次のコマンドを実行します。
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
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
 
Exchange 管理センターのアイテム保持ポリシーの詳細については、以下を参照してください。
- [保持タグおよびアイテム保持ポリシー](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [メールボックスにアイテム保持ポリシーを適用する](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [アイテム保持タグの追加または削除](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [メールボックスに適用されている保留の種類を特定する方法](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)

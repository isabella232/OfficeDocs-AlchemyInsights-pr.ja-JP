---
title: アーカイブ メールボックスへのメール メッセージの移動
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 2147c70f64087bf95fc4e39c193caeac3b2c5361
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660387"
---
アーカイブ メールボックスにアイテムを整理すると、問題が発生します。次の手順を実行したことを確認してください。
  
1. **[アーカイブ メールボックス]** が有効になっていることを確認します。そうでない場合は、[この記事](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)の手順を使用して、アーカイブ メールボックスを有効にします。 
    
2. Exchange 管理センターで、**[コンプライアンス管理]** の下の **[保持タグ]** を選択し、必要な**保存の有効期限**を含む **[アーカイブに移動]** アクションを使用した**保持タグ**を作成します。
    
3. Exchange 管理センターで、**[アイテム保持ポリシー]** を選択し、**[アイテム保持ポリシー]** を作成し、そのポリシーに **[アーカイブに移動]** 保持タグを追加します。 
    
4. 特定のユーザーのメールボックスに[アイテム保持ポリシーを割り当て](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)ます。同じポリシーは、**プライマリ**および**アーカイブ** メールボックスにも適用されます。 
    
これでユーザーのメールボックスには、アイテムをアーカイブ メールボックスに移動するアーカイブ ポリシーが用意されました。場合によっては、強制的に管理フォルダー用アシスタント (MFA) を実行して、新しい設定をユーザーのメールボックスに適用する必要があります。[EXO PowerShell に接続された](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)状態で次のコマンドを実行し、特定のメールボックスに対して管理フォルダー用アシスタントを起動します。 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

アーカイブ ポリシーの設定の詳細については、[メールボックスのアーカイブと削除ポリシーの設定](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)に関するページを参照してください。
  


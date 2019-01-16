---
title: アーカイブ メールボックスに電子メール メッセージを移動
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28298264"
---
アーカイブ メールボックスにアイテムをアーカイブする問題が発生します。次の手順を実行することを確認します。
  
1. の**アーカイブ メールボックス**が有効であることを確認します。それ以外の場合は、[この資料](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes)の手順を使用して、アーカイブ メールボックスを有効にします。 
    
2. Exchange 管理センターで、**コンプライアンスの管理**下にある**保持タグ**を選択して、**アーカイブに移動する**操作が必要な**保有期間**が含まれている**保持タグ**を作成します。
    
3. Exchange 管理センターで、**リテンション ・ ポリシー**を選択を選択し、**リテンション ・ ポリシー**を作成するタグを追加、**アーカイブに移動する**保持ポリシーにします。 
    
4. 特定のユーザーのメールボックスに[保持ポリシーを割り当てる](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)を。同じポリシーは、**主**と**アーカイブ先**のメールボックスの両方に適用されます。 
    
ユーザーのメールボックスがアーカイブ メールボックスにアイテムを移動するのには、アーカイブ ポリシーできました。強制的に、管理フォルダー アシスタント (MFA) を実行し、ユーザーのメールボックスに新しい設定を適用する必要がある場合があります。[EXO PowerShell に接続されて](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)いるときに、管理フォルダー アシスタントに特定のメールボックスを開始する次のコマンドを実行します。 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

アーカイブ ポリシーを設定する方法については、[メールボックスのアーカイブと削除ポリシーを設定](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)するを参照します。
  


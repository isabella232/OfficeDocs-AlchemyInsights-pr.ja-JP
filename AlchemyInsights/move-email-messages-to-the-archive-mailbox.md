---
title: アーカイブ メールボックスへのメール メッセージの移動
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418324"
---
# <a name="move-email-to-the-archive-mailbox"></a>メールをアーカイブメールボックスに移動する
 
1. **アーカイブメールボックス**が有効になっていることを確認します。 それ以外の場合は、[この記事](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)の手順を使用してアーカイブメールボックスを有効にします。

2. アーカイブメールボックスにメッセージを自動的にアーカイブするには、[**アーカイブに移動**する] アクションを持つ保持タグを、 **mailbox (default) タグ全体に自動的に適用**するように設定する必要があります。 タグ: [Archive Default タグ](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0)を作成するには、以下の手順を使用します。
    
3. 次に、アイテム保持ポリシーに**アーカイブ**タグを追加します。 Exchange 管理センターで [**アイテム保持ポリシー** >] を選択し、[**アーカイブに移動する] タグ**を [ポリシー >**保存**] に追加します。 
    
4. 次に[、アイテム保持ポリシー](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)を特定のユーザーのメールボックスに割り当てます。 同じポリシーが**プライマリ**メールボックスと**アーカイブ**メールボックスの両方に適用されます。 
    
管理フォルダーアシスタント (MFA) を強制的に実行して、新しい設定をユーザーのメールボックスに適用する必要がある場合があります。 [exo PowerShell に接続して](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)いるときに、特定のメールボックスの管理フォルダーアシスタントを開始するには、次のコマンドを実行します。 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

アーカイブポリシーの設定の詳細については、「[メールボックスのアーカイブおよび削除ポリシーをセットアップする](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)」を参照してください。
  


---
title: "\"アクセスが拒否されました\" メッセージのトラブルシューティング"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704899"
---
# <a name="troubleshoot-access-denied-messages"></a>"アクセスが拒否されました" メッセージのトラブルシューティング

ユーザーが SharePoint の共有フォルダーにアクセスしようとしたときに「アクセスが拒否されました」メッセージを受け取った場合、サイト コレクション管理者が「制限付きアクセスのユーザーのアクセス許可ロックダウン モード」を有効にしている可能性があります。これを無効にするには、次の手順を実行します。 
  
1. サイトを参照して、[設定] アイコンをクリックし、[**サイト設定**] をクリックします。
    
2. [**サイト コレクションの管理**] で、[**サイト コレクションの機能**] をクリックします。
    
3. [**制限付きアクセスのユーザーのアクセス許可ロックダウン モード**] の横にある [**非アクティブ化**] をクリックします。
    
"アクセスが拒否されました" メッセージは、サイトが発行サイトである場合に共有フォルダーを参照しようとしたときにも発生します。詳細については、[共有フォルダーにアクセスしようとしたときに表示される "アクセスが拒否されました" エラー メッセージに関する記事](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)を参照してください。
  
ユーザーがアクセス依頼を表示しようとしたときに "アクセスが拒否されました" メッセージを受け取った場合、そのユーザーをサイト コレクション管理者またはサイトの所有者グループのメンバーとして追加する必要があります。詳細については、[アクセス依頼リストにアクセスしようとしたときに表示される "アクセスが拒否されました" エラー メッセージに関する記事](https://go.microsoft.com/fwlink/?linkid=2004220)を参照してください。
  
ユーザーがオンプレミスの Active Directory から削除され、再度追加された後に "アクセスが拒否されました" メッセージを受け取った場合は、[ユーザー アカウントを Microsoft 365 に同期しようとしたときに表示される "アクセスが拒否されました" エラー メッセージに関する記事](https://go.microsoft.com/fwlink/?linkid=2004318)を参照してください。
  


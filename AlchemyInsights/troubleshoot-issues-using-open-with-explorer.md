---
title: '[エクスプローラーで開く] を使用して問題のトラブルシューティングを行う'
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 9b2abe01a47d39812988d62b6f010a8933fad33e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929214"
---
# <a name="fix-problems-with-open-with-explorer"></a>[エクスプローラーで開く] を使用して問題を解決します

SharePoint または OneDrive のドキュメント ライブラリを開くときの一般的な問題を **[エクスプローラーで開く]** コマンドを使用して解決します。 
  
- Internet Explorer 10 または Internet Explorer 11 を使用します。**[エクスプローラーで開く]** は Microsoft Edge、Google Chrome、Firefox などとは互換性がありません。Internet Explorer 以外のブラウザーでは **[エクスプローラーで開く]** は無効です。 
    
- **[エクスプローラーで開く]** は SharePoint ライブラリのモダン エクスペリエンスでは利用できません。代わりに、**[エクスプローラーで表示]** を使用します。**[表示オプション]** \> **[エクスプローラーで表示]** と選択します。[エクスプローラーで表示] は Microsoft Edge、Google Chrome、Firefox などとは互換性がありません。**[エクスプローラーで表示]** は Internet Explorer でのみ利用できます。 
    
- WebClient サービスが実行されていることを確認します。Windows の検索ボックスに「実行」と入力し、「ファイル名を指定して実行」デスクトップ アプリを選択します。services.msc と入力して Enter を押します。WebClient サービスまで下方向にスクロールし、**[状態]** 列に [実行中] と表示されていることを確認します。表示されていない場合には、このサービスをダブルクリックし、**[開始]**、**[OK]** の順にクリックします (最初に、**[手動]** または **[自動]** を **[スタートアップの種類]** ボックスで選択してサービスを有効にしなければならない場合もあります)。 
    
> [!NOTE]
> エクスプローラーでライブラリを開くと、一度に複数のファイルやフォルダーをコピーまたは移動する必要がある場合に便利ですが、ライブラリ内で定期的に作業する場合は、同期することをお勧めします。エクスプローラーで開く場合に関する問題のトラブルシューティングについては、「[エクスプローラーで開く](https://go.microsoft.com/fwlink/?linkid=871665)」を参照してください。同期の設定については、「[新しい OneDrive 同期クライアントを使用して SharePoint ファイルを同期する](https://go.microsoft.com/fwlink/?linkid=871666)」を参照してください。
  
詳しくは、「[[エクスプローラーで開く] コマンドを使用して、SharePoint Online の問題をトラブルシューティングする方法](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)」という記事をご覧ください。 
  


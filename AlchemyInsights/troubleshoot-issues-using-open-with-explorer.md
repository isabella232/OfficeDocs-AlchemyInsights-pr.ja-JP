---
title: エクスプ ローラーを開くを使用して、問題のトラブルシューティングを行う
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: c95f07b9fb7251442577c014e4005dbe3f92ceb4
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661756"
---
# <a name="fix-problems-with-open-with-explorer"></a>エクスプ ローラーを開いた状態で問題を修正します。

SharePoint または**エクスプ ローラーで開く**コマンドを使用して OneDrive でドキュメント ライブラリを開くときの一般的な問題を修正します。 
  
- Internet Explorer 10 または 11 の Internet Explorer を使用します。**エクスプ ローラーで開く**と互換性のない Microsoft エッジ、Google Chrome、Firefox と他のユーザーです。**エクスプ ローラーで開く**は、Internet Explorer 以外のすべてのブラウザーで無効になっています。 
    
- **エクスプ ローラーで開く**は SharePoint ライブラリの最近の経験では利用可能ではありません。**ファイル エクスプ ローラーでビュー**を使用してください。**表示オプション**を選択\>**ファイルのエクスプ ローラーで表示**します。ファイル エクスプ ローラーでのビューは、マイクロソフトのエッジ、Google Chrome、Firefox と他のユーザーとの互換性はありません。**ファイル エクスプ ローラー ビュー**で Internet Explorer でのみ使用します。 
    
- WebClient サービスが実行されていることを確認します。Windows の検索ボックスでこれを実行すると、型の実行のデスクトップ アプリケーションを選択、services.msc を入力し、Enter キーを押します。WebClient サービスまでスクロールし、[**状態**] 列になります。 が表示されるかどうかを確認しない場合、サービスをダブルクリックして**開始**] をクリック、[ **OK**] をクリックします。(まず、[**スタートアップの種類**] ボックスに**手動**または**自動**のいずれかを選択することでサービスを有効にする必要があります)。 
    
> [!NOTE]
> ファイル エクスプ ローラーで、ライブラリを開くときは、コピーまたは、1 回だけですが、ライブラリで定期的に作業を行う場合に、複数のファイルとフォルダーを移動する必要がある場合に便利ですが、同期することお勧めします。ファイル エクスプ ローラーで開くときの問題のトラブルシューティングを行うには、[エクスプ ローラーで開く](https://go.microsoft.com/fwlink/?linkid=871665)を参照してください。同期の設定に関する情報は、[新しい OneDrive 同期クライアントと同期 SharePoint ファイル](https://go.microsoft.com/fwlink/?linkid=871666)を参照してください。
  
[SharePoint Online での問題をトラブルシューティングするのには [開くとエクスプ ローラー] コマンドを使用する方法](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)の詳細についての資料を参照してください。 
  


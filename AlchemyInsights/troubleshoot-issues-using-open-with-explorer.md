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
ms.openlocfilehash: 5be8a8f9f67939c7e2671855da259818269d9299
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297928"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="54208-102">エクスプ ローラーを開いた状態で問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="54208-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="54208-103">SharePoint または**エクスプ ローラーで開く**コマンドを使用して OneDrive でドキュメント ライブラリを開くときの一般的な問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="54208-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="54208-p101">Internet Explorer 10 または 11 の Internet Explorer を使用します。**エクスプ ローラーで開く**と互換性のない Microsoft エッジ、Google Chrome、Firefox と他のユーザーです。**エクスプ ローラーで開く**は、Internet Explorer 以外のすべてのブラウザーで無効になっています。</span><span class="sxs-lookup"><span data-stu-id="54208-p101">Use Internet Explorer 10 or Internet Explorer 11. **Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others. **Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="54208-p102">**エクスプ ローラーで開く**は SharePoint ライブラリの最近の経験では利用可能ではありません。**ファイル エクスプ ローラーでビュー**を使用してください。**表示オプション**を選択\>**ファイルのエクスプ ローラーで表示**します。ファイル エクスプ ローラーでのビューは、マイクロソフトのエッジ、Google Chrome、Firefox と他のユーザーとの互換性はありません。**ファイル エクスプ ローラー ビュー**で Internet Explorer でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="54208-p102">**Open with Explorer** is not available in the modern experience for SharePoint libraries. Use **View in File Explorer** instead. Select **View options** \> **View in File Explorer**. View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others. **View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="54208-p103">WebClient サービスが実行されていることを確認します。Windows の検索ボックスでこれを実行すると、型の実行のデスクトップ アプリケーションを選択、services.msc を入力し、Enter キーを押します。WebClient サービスまでスクロールし、[**状態**] 列になります。 が表示されるかどうかを確認しない場合、サービスをダブルクリックして**開始**] をクリック、[ **OK**] をクリックします。(まず、[**スタートアップの種類**] ボックスに**手動**または**自動**のいずれかを選択することでサービスを有効にする必要があります)。</span><span class="sxs-lookup"><span data-stu-id="54208-p103">Make sure the WebClient service is running. In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter. Scroll down to the WebClient service and make sure the **Status** column displays "Running." If it doesn't, double-click the service, click **Start**, and then click **OK**. (You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="54208-p104">ファイル エクスプ ローラーで、ライブラリを開くときは、コピーまたは、1 回だけですが、ライブラリで定期的に作業を行う場合に、複数のファイルとフォルダーを移動する必要がある場合に便利ですが、同期することお勧めします。ファイル エクスプ ローラーで開くときの問題のトラブルシューティングを行うには、[エクスプ ローラーで開く](https://go.microsoft.com/fwlink/?linkid=871665)を参照してください。同期の設定に関する情報は、[新しい OneDrive 同期クライアントと同期 SharePoint ファイル](https://go.microsoft.com/fwlink/?linkid=871666)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54208-p104">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it. To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="54208-120">[SharePoint Online での問題をトラブルシューティングするのには [開くとエクスプ ローラー] コマンドを使用する方法](https://support.office.com/en-us/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)の詳細についての資料を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54208-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/en-us/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  


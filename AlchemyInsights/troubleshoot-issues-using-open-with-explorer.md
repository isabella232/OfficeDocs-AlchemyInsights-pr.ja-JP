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
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742738"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="62d8d-102">[エクスプローラーで開く] を使用して問題を解決します</span><span class="sxs-lookup"><span data-stu-id="62d8d-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="62d8d-103">SharePoint または OneDrive のドキュメント ライブラリを開くときの一般的な問題を **[エクスプローラーで開く]** コマンドを使用して解決します。</span><span class="sxs-lookup"><span data-stu-id="62d8d-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="62d8d-p101">Internet Explorer 10 または Internet Explorer 11 を使用します。**[エクスプローラーで開く]** は Microsoft Edge、Google Chrome、Firefox などとは互換性がありません。Internet Explorer 以外のブラウザーでは **[エクスプローラーで開く]** は無効です。</span><span class="sxs-lookup"><span data-stu-id="62d8d-p101">Use Internet Explorer 10 or Internet Explorer 11. **Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others. **Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="62d8d-p102">**[エクスプローラーで開く]** は SharePoint ライブラリのモダン エクスペリエンスでは利用できません。代わりに、**[エクスプローラーで表示]** を使用します。**[表示オプション]** \> **[エクスプローラーで表示]** と選択します。[エクスプローラーで表示] は Microsoft Edge、Google Chrome、Firefox などとは互換性がありません。**[エクスプローラーで表示]** は Internet Explorer でのみ利用できます。</span><span class="sxs-lookup"><span data-stu-id="62d8d-p102">**Open with Explorer** is not available in the modern experience for SharePoint libraries. Use **View in File Explorer** instead. Select **View options** \> **View in File Explorer**. View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others. **View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="62d8d-p103">WebClient サービスが実行されていることを確認します。Windows の検索ボックスに「実行」と入力し、「ファイル名を指定して実行」デスクトップ アプリを選択します。services.msc と入力して Enter を押します。WebClient サービスまで下方向にスクロールし、**[状態]** 列に [実行中] と表示されていることを確認します。表示されていない場合には、このサービスをダブルクリックし、**[開始]**、**[OK]** の順にクリックします (最初に、**[手動]** または **[自動]** を **[スタートアップの種類]** ボックスで選択してサービスを有効にしなければならない場合もあります)。</span><span class="sxs-lookup"><span data-stu-id="62d8d-p103">Make sure the WebClient service is running. In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter. Scroll down to the WebClient service and make sure the **Status** column displays "Running." If it doesn't, double-click the service, click **Start**, and then click **OK**. (You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="62d8d-p104">エクスプローラーでライブラリを開くと、一度に複数のファイルやフォルダーをコピーまたは移動する必要がある場合に便利ですが、ライブラリ内で定期的に作業する場合は、同期することをお勧めします。エクスプローラーで開く場合に関する問題のトラブルシューティングについては、「[エクスプローラーで開く](https://go.microsoft.com/fwlink/?linkid=871665)」を参照してください。同期の設定については、「[新しい OneDrive 同期クライアントを使用して SharePoint ファイルを同期する](https://go.microsoft.com/fwlink/?linkid=871666)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62d8d-p104">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it. To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="62d8d-120">詳しくは、「[[エクスプローラーで開く] コマンドを使用して、SharePoint Online の問題をトラブルシューティングする方法](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)」という記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="62d8d-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  


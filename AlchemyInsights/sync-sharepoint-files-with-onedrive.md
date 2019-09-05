---
title: SharePoint Online での「エクスプローラーで開く」問題のトラブルシューティング
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 73583b3b27143c708a4cc993cdff94a33131ab52
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36743098"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="ddcb6-102">SharePoint Online での「エクスプローラーで開く」問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="ddcb6-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="ddcb6-103">[エクスプローラーで開く] コマンドを使用すると、エクスプローラーのローカル インスタンスが開いて、SharePoint サイトをホストするサーバーのフォルダー構造が表示されます。</span><span class="sxs-lookup"><span data-stu-id="ddcb6-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="ddcb6-104">そのため、[新しい OneDrive 同期クライアントを使用して SharePoint ファイルを同期する](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>ことをお勧めします。これにより、[ファイル オンデマンド](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)が可能になります。そうすることで、自分のファイルにローカル アクセスできるようになりパフォーマンスが向上します。</span><span class="sxs-lookup"><span data-stu-id="ddcb6-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="ddcb6-105">新しい OneDrive 同期クライアントを使用せずに、エクスプローラー ビューを使用する場合は、次の記事に示された手順とベスト プラクティスに従ってください。</span><span class="sxs-lookup"><span data-stu-id="ddcb6-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- <span data-ttu-id="ddcb6-106">[[エクスプローラーで開く] コマンドを使用して SharePoint Online の問題をトラブルシューティングする方法](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)</span><span class="sxs-lookup"><span data-stu-id="ddcb6-106">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span>

- <span data-ttu-id="ddcb6-107">[[エクスプローラーで開く] を使用してライブラリ ファイルをコピーまたは移動する](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span><span class="sxs-lookup"><span data-stu-id="ddcb6-107">[Copy or move library files by using Open with Explorer](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span></span>

> [!Note]  
> <span data-ttu-id="ddcb6-108">**[エクスプローラーで開く]** ボタンは、新しいライブラリ エクスペリエンスには表示されません。</span><span class="sxs-lookup"><span data-stu-id="ddcb6-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="ddcb6-109">右上にある **[表示]** ドロップダウン (このドロップダウンの名前は、現在のビューによって変化します) をクリックして、**[エクスプローラーで表示]** をクリックしてください。</span><span class="sxs-lookup"><span data-stu-id="ddcb6-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="ddcb6-110">SharePoint の [エクスプローラーで開く] は ActiveX コントロールを使用するため、Internet Explorer 10 または 11 のみでサポートされます。</span><span class="sxs-lookup"><span data-stu-id="ddcb6-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="ddcb6-111">[エクスプローラーで開く] は、Microsoft Edge、Google Chrome、Mozilla FireFox を使用した場合の Windows、または Mac プラットフォームでは機能しません。</span><span class="sxs-lookup"><span data-stu-id="ddcb6-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="ddcb6-112">そのため、[エクスプローラー ビュー] オプションが灰色表示になることがあります。</span><span class="sxs-lookup"><span data-stu-id="ddcb6-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="ddcb6-113">[SharePoint のリボン ボタンが使用不可または灰色表示になる理由](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)。</span><span class="sxs-lookup"><span data-stu-id="ddcb6-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  


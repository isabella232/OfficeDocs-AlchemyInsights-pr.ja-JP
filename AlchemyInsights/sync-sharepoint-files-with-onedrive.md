---
title: SharePoint Online での「エクスプローラーで開く」問題のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ba9f11da5c35c3681e9bd5ceaf13233fe8b80fc9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737310"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="06a6e-102">SharePoint Online での「エクスプローラーで開く」問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="06a6e-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="06a6e-103">[新しい OneDrive 同期クライアントを使用して SharePoint ファイルを同期する](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)ことをお勧めします。これにより、[ファイル オンデマンド](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)が可能になります。そうすることで、自分のファイルにローカル アクセスできるようになりパフォーマンスが向上します。</span><span class="sxs-lookup"><span data-stu-id="06a6e-103">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>

<span data-ttu-id="06a6e-104">[エクスプローラーで開く] の問題をトラブルシューティングするには、次の記事の手順およびベスト プラクティスに従ってください。</span><span class="sxs-lookup"><span data-stu-id="06a6e-104">To troubleshoot Open with Explorer issues, follow the steps and best practices in the following articles:</span></span>

- <span data-ttu-id="06a6e-105">[[エクスプローラーで開く] コマンドを使用して SharePoint Online の問題をトラブルシューティングする方法](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)</span><span class="sxs-lookup"><span data-stu-id="06a6e-105">[How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)</span></span>
- <span data-ttu-id="06a6e-106">[[エクスプローラーで開く] を使用してライブラリ ファイルをコピーまたは移動する](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span><span class="sxs-lookup"><span data-stu-id="06a6e-106">[Copy or move library files by using Open with Explorer](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span></span>

> <span data-ttu-id="06a6e-107">**注:** </span><span class="sxs-lookup"><span data-stu-id="06a6e-107">**Note:**</span></span>
>- <span data-ttu-id="06a6e-108">[エクスプローラーで開く] は、Internet Explorer 10 または 11 でのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="06a6e-108">Open with Explorer is only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="06a6e-109">[エクスプローラーで開く] は、Microsoft Edge、Google Chrome、Mozilla FireFox を使用した場合の Windows、または Mac プラットフォームでは機能しません。</span><span class="sxs-lookup"><span data-stu-id="06a6e-109">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="06a6e-110">そのため、[エクスプローラー ビュー] オプションが灰色表示になることがあります。</span><span class="sxs-lookup"><span data-stu-id="06a6e-110">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
>- <span data-ttu-id="06a6e-111">[エクスプローラーで開く] ボタンは、新しいライブラリ エクスペリエンスには表示されません。</span><span class="sxs-lookup"><span data-stu-id="06a6e-111">The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="06a6e-112">右上にある **[表示]** ドロップダウン (このドロップダウンの名前は、現在のビューによって変化します) をクリックして、**[エクスプローラーで表示]** をクリックしてください。</span><span class="sxs-lookup"><span data-stu-id="06a6e-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

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
ms.custom:
- "6462"
- "9003546"
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ea93bb6f3cbbc3424f5e006ffac482a7445c8164
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086053"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="3989a-102">SharePoint Online での「エクスプローラーで開く」問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="3989a-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="3989a-103">次の記事の手順とベスト プラクティスに従ってください。</span><span class="sxs-lookup"><span data-stu-id="3989a-103">Follow the steps and best practices in the following articles:</span></span>

- <span data-ttu-id="3989a-104">[[エクスプローラーで開く] コマンドを使用して SharePoint Online の問題をトラブルシューティングする方法](https://docs.microsoft.com/sharepoint/troubleshoot/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)</span><span class="sxs-lookup"><span data-stu-id="3989a-104">[How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/troubleshoot/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)</span></span>

- <span data-ttu-id="3989a-105">[[エクスプローラーで開く] を使用してライブラリ ファイルをコピーまたは移動する](https://support.microsoft.com/office/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="3989a-105">[Copy or move library files by using Open with Explorer](https://support.microsoft.com/office/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2?ui=en-us&rs=en-us&ad=us)</span></span>

> [!NOTE]
- <span data-ttu-id="3989a-106">同期によりファイルへのローカルアクセスが許可され、最高のパフォーマンスが提供されるため、SharePoint ファイルを[ファイル オンデマンド](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us)を提供する[新しい OneDrive 同期クライアント](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us)と同期することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="3989a-106">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) which provides [Files On-Demand](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) because the synchronization grants local access to your files and offers the best performance.</span></span>

- <span data-ttu-id="3989a-107">**[エクスプローラーで開く]** は、Internet Explorer 11 でのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="3989a-107">**Open with Explorer** is only supported in Internet Explorer 11.</span></span> <span data-ttu-id="3989a-108">詳細については、[IE 11 のサポート終了とMicrosoft 365 アプリ](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3989a-108">For more information, see [end of support for IE11 with Microsoft 365 Apps](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)).</span></span> <span data-ttu-id="3989a-109">**[エクスプローラーで開く]** は、Microsoft Edge、Google Chrome、Mozilla FireFox を使用した場合の Windows、または Mac プラットフォームでは機能しません。</span><span class="sxs-lookup"><span data-stu-id="3989a-109">**Open with Explorer** doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="3989a-110">そのため、**[エクスプローラー ビュー]** オプションが灰色表示になることがあります。</span><span class="sxs-lookup"><span data-stu-id="3989a-110">Due to this reason, the **Explorer View** option may be grayed out.</span></span> 

- <span data-ttu-id="3989a-111">**[エクスプローラーで開く]** ボタンは、新しいライブラリ エクスペリエンスには表示されません。</span><span class="sxs-lookup"><span data-stu-id="3989a-111">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="3989a-112">右上にある **[表示]** ドロップダウン (このドロップダウンの名前は、現在のビューによって変化します) をクリックして、**[エクスプローラーで表示]** をクリックしてください。</span><span class="sxs-lookup"><span data-stu-id="3989a-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>


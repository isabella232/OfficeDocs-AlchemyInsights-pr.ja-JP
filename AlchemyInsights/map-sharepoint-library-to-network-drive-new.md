---
title: SharePoint ライブラリをネットワーク ドライブにマップする
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 7bb1f7d1b77ec5850109c9553ddfd894b3823946
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35174448"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="ea588-102">SharePoint ライブラリをネットワーク ドライブにマップする</span><span class="sxs-lookup"><span data-stu-id="ea588-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="ea588-103">ライブラリをネットワーク ドライブとしてマップすることは一時的であり、Internet Explorer でのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="ea588-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="ea588-104">そのため、セッションが期限切れになることを防ぐには、Internet Explorer で SharePoint サイトを開き、[サインインした状態を維持] を選択する操作をときどき行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="ea588-104">Mapping a SharePoint document library to a network drive is temporary. You must occasionally open the SharePoint site in Internet Explorer and select Stay signed in to prevent the session from expiring.</span></span> <span data-ttu-id="ea588-105">ライブラリをマップする代わりに、 [ファイル オンデマンド](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)機能が備わった[新しい OneDrive 同期クライアントを使用して SharePoint ファイルを同期](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>します。</span><span class="sxs-lookup"><span data-stu-id="ea588-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="ea588-106">OneDrive 内のすべてのファイルに、ローカル記憶域を使用することなくアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="ea588-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="ea588-107">[新しい OneDrive 同期クライアントを使用](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)する代わりに、ドライブをマップする方法を選択する場合は、次の記事の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="ea588-107">If you choose to map a drive instead of[using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="ea588-108">**マップされたネットワーク ドライブを構成しトラブルシューティングする方法**</span><span class="sxs-lookup"><span data-stu-id="ea588-108">**How to configure and troubleshoot mapped network drives**</span></span>


- <span data-ttu-id="ea588-109">[マップされたネットワーク ドライブの構成とトラブルシューティング](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US)。</span><span class="sxs-lookup"><span data-stu-id="ea588-109">[Configure and troubleshoot mapped network drives](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US)</span></span>

<span data-ttu-id="ea588-110">注: Windows 8 または Windows 7 で実行する Internet Explorer 10 でドライブをマップする際に "アクセスが拒否されました" または "パスにアクセスできません" というメッセージが表示される場合は、この修正プログラムをインストールして問題を解決してください。</span><span class="sxs-lookup"><span data-stu-id="ea588-110">NOTE:  For Internet Explorer 10 with Windows 8 or Windows 7 that receive "Access denied" or "Path is not accessible" when mapping a drive, install this hotfix to resolve this problem.</span></span> <span data-ttu-id="ea588-111">詳細については、「[Internet Explorer 10 をインストールした後にエクスプローラーで SharePoint ドキュメント ライブラリを開くか、SharePoint ドキュメント ライブラリにネットワーク ドライブを割り当てると、エラーが発生する](https://support.microsoft.com/help/2846960)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea588-111">Go to [Error when you open a SharePoint Document Library in Windows Explorer or map a network drive to the library after you install Internet Explorer 10](https://support.microsoft.com/help/2846960).</span></span>

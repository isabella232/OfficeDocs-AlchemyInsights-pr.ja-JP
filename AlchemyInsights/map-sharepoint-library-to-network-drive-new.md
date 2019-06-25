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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35174448"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="0bdec-102">SharePoint ライブラリをネットワーク ドライブにマップする</span><span class="sxs-lookup"><span data-stu-id="0bdec-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="0bdec-103">ライブラリをネットワークドライブとしてマッピングすることは一時的で、Internet Explorer を使用する場合にのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="0bdec-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="0bdec-104">Internet Explorer で SharePoint サイトを開き、[サインイン状態を維持する] を選択して、セッションが期限切れにならないようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0bdec-104">You must occasionally open the SharePoint site in Internet Explorer and select "Stay signed in" to prevent the session from expiring.</span></span> <span data-ttu-id="0bdec-105">代わりに、[新しい OneDrive 同期クライアント](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>を使用して SharePoint ファイルを同期します。これにより、[オンデマンドでファイル](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)が提供されます。</span><span class="sxs-lookup"><span data-stu-id="0bdec-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="0bdec-106">ローカル記憶域を使用せずに OneDrive のすべてのファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="0bdec-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="0bdec-107">[新しい OneDrive 同期クライアントを使用](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)する代わりにドライブをマップすることを選択した場合は、以下の記事の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="0bdec-107">If you choose to map a drive instead of[using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="0bdec-108">**マップされたネットワークドライブを構成およびトラブルシューティングする方法**</span><span class="sxs-lookup"><span data-stu-id="0bdec-108">**How to configure and troubleshoot mapped network drives**</span></span>


- <span data-ttu-id="0bdec-109">マップされた[ネットワークドライブを構成し、トラブルシューティングを行う](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US)。</span><span class="sxs-lookup"><span data-stu-id="0bdec-109">[Configure and to troubleshoot mapped network drives](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

<span data-ttu-id="0bdec-110">注: ドライブのマッピング時に "アクセスが拒否されました" または "パスにアクセスできません" を受け取る Windows 8 または Windows 7 の Internet Explorer 10 の場合は、この修正プログラムをインストールしてこの問題を解決してください。</span><span class="sxs-lookup"><span data-stu-id="0bdec-110">NOTE:  For Internet Explorer 10 with Windows 8 or Windows 7 that receive "Access denied" or "Path is not accessible" when mapping a drive, install this hotfix to resolve this problem.</span></span> <span data-ttu-id="0bdec-111">[Internet explorer 10 をインストールした後、Windows Explorer で SharePoint ドキュメントライブラリを開くとき、またはネットワークドライブをライブラリに割り当てるとき](https://support.microsoft.com/help/2846960)に、エラーに移動します。</span><span class="sxs-lookup"><span data-stu-id="0bdec-111">Go to [Error when you open a SharePoint Document Library in Windows Explorer or map a network drive to the library after you install Internet Explorer 10](https://support.microsoft.com/help/2846960).</span></span>

---
title: ビデオの再生に使用される CDN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: 489e92ad8fb38ff6f62db3cb65bfd6d329c63490
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2020
ms.locfileid: "43791318"
---
# <a name="cdn-used-for-video-playback"></a><span data-ttu-id="7e4b0-102">ビデオの再生に使用される CDN</span><span class="sxs-lookup"><span data-stu-id="7e4b0-102">CDN used for video playback</span></span>

<span data-ttu-id="7e4b0-103">Stream および外部アプリからのライブ イベントや、Yammer または Teams からのデバイス ライブ イベントには、自動的に Azure CDN が使用されます。</span><span class="sxs-lookup"><span data-stu-id="7e4b0-103">Live events from Stream and External app or device live events from Yammer/Teams will automatically use Azure CDN.</span></span> <span data-ttu-id="7e4b0-104">Stream にアップロードしたオンデマンドのビデオは、まだ、再生の際に Azure CDN が使用されません。</span><span class="sxs-lookup"><span data-stu-id="7e4b0-104">On-demand videos uploaded to Stream don't yet use Azure CDN for playback.</span></span> <span data-ttu-id="7e4b0-105">Stream のライブ以外のビデオは、テナントの地理的リージョン内でテナントに関連付けられた Azure Media Services 配信元サーバーから再生されます。</span><span class="sxs-lookup"><span data-stu-id="7e4b0-105">Non-live videos in Stream are played back from the Azure Media Services origin server associated with your tenant in your tenant's geographic region.</span></span> <span data-ttu-id="7e4b0-106">詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e4b0-106">For more information, see:</span></span>

- [<span data-ttu-id="7e4b0-107">ビデオの再生に使用される CDN</span><span class="sxs-lookup"><span data-stu-id="7e4b0-107">CDN used for video playback</span></span>](https://docs.microsoft.com/ja-JP/stream/network-overview#cdn-used-for-video-playback)

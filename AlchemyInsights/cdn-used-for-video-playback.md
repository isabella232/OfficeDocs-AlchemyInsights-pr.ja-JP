---
title: ビデオの再生に使用される CDN
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: d9c5f8f586e7f5aa079b28584375516ec8401ca7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819373"
---
# <a name="cdn-used-for-video-playback"></a><span data-ttu-id="b0802-102">ビデオの再生に使用される CDN</span><span class="sxs-lookup"><span data-stu-id="b0802-102">CDN used for video playback</span></span>

<span data-ttu-id="b0802-103">Stream および外部アプリからのライブ イベントや、Yammer または Teams からのデバイス ライブ イベントには、自動的に Azure CDN が使用されます。</span><span class="sxs-lookup"><span data-stu-id="b0802-103">Live events from Stream and External app or device live events from Yammer/Teams will automatically use Azure CDN.</span></span> <span data-ttu-id="b0802-104">Stream にアップロードしたオンデマンドのビデオは、まだ、再生の際に Azure CDN が使用されません。</span><span class="sxs-lookup"><span data-stu-id="b0802-104">On-demand videos uploaded to Stream don't yet use Azure CDN for playback.</span></span> <span data-ttu-id="b0802-105">Stream のライブ以外のビデオは、テナントの地理的リージョン内でテナントに関連付けられた Azure Media Services 配信元サーバーから再生されます。</span><span class="sxs-lookup"><span data-stu-id="b0802-105">Non-live videos in Stream are played back from the Azure Media Services origin server associated with your tenant in your tenant's geographic region.</span></span> <span data-ttu-id="b0802-106">詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0802-106">For more information, see:</span></span>

- [<span data-ttu-id="b0802-107">ビデオの再生に使用される CDN</span><span class="sxs-lookup"><span data-stu-id="b0802-107">CDN used for video playback</span></span>](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)

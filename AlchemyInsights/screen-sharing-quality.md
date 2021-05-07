---
title: 画面共有の品質
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11061"
- "11062"
- "9002254"
- "9002536"
ms.openlocfilehash: 0832f886d3f5c0bfbfe138647403e4e215deaacb
ms.sourcegitcommit: d822377ec76adf9ef6d13bc761a16c9900a3e7cb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2021
ms.locfileid: "52125836"
---
# <a name="screen-sharing-quality"></a><span data-ttu-id="d2866-102">画面共有の品質</span><span class="sxs-lookup"><span data-stu-id="d2866-102">Screen sharing quality</span></span>

<span data-ttu-id="d2866-103">ほとんどの場合、画面共有の品質の問題は、クライアント側からの帯域幅が限られていることに起因します。</span><span class="sxs-lookup"><span data-stu-id="d2866-103">In most cases quality issues with Screen Sharing comes down to limited bandwidth from the client side.</span></span>  <span data-ttu-id="d2866-104">帯域幅が制限されていない場合、Teams は、最大 1080p のビデオ解像度、最大 30fps のビデオと 15fps のコンテンツ、およびハイファイ オーディオなど、メディア品質を最適化します。</span><span class="sxs-lookup"><span data-stu-id="d2866-104">Where bandwidth isn't limited, Teams optimizes media quality, including up to 1080p video resolution, up to 30fps for video and 15fps for content, and high-fidelity audio.</span></span>

<span data-ttu-id="d2866-105">Teams は常に帯域幅の使用率を控えめにし、1.2 Mbps 以下で HD ビデオ品質を提供できます。</span><span class="sxs-lookup"><span data-stu-id="d2866-105">Teams is always conservative on bandwidth utilization and can deliver HD video quality in under 1.2Mbps.</span></span> <span data-ttu-id="d2866-106">各オーディオ/ビデオ通話または会議の実際の帯域幅の消費量は、ビデオレイアウト、ビデオ解像度、1 秒あたりのビデオ フレームなどの要因によって異なります。</span><span class="sxs-lookup"><span data-stu-id="d2866-106">The actual bandwidth consumption in each audio/video call or meeting vary based on factors such as video layout, video resolution, and video frames per second.</span></span> <span data-ttu-id="d2866-107">より多くの帯域幅が利用可能になると、最高のエクスペリエンスを提供するために品質と使用率を増加させるようになっています。</span><span class="sxs-lookup"><span data-stu-id="d2866-107">When more bandwidth is available, quality and usage increase to deliver the best experience.</span></span> <span data-ttu-id="d2866-108">この表では、Teams がどのように帯域幅を使用するかについて説明しています。</span><span class="sxs-lookup"><span data-stu-id="d2866-108">This table describes how Teams uses bandwidth:</span></span>

<span data-ttu-id="d2866-109">**帯域 (上り/下り) のシナリオ**</span><span class="sxs-lookup"><span data-stu-id="d2866-109">**Bandwidth(up/down) Scenarios**</span></span>

- <span data-ttu-id="d2866-110">30 kbps のピアツーピア音声通話</span><span class="sxs-lookup"><span data-stu-id="d2866-110">30 kbps Peer-to-peer audio calling</span></span>

- <span data-ttu-id="d2866-111">130 kbps ピアツーピア音声通話と画面共有</span><span class="sxs-lookup"><span data-stu-id="d2866-111">130 kbps Peer-to-peer audio calling and screen sharing</span></span>

- <span data-ttu-id="d2866-112">30 fps で 360 p の 500 kbps でピアツーピア品質ビデオ通話</span><span class="sxs-lookup"><span data-stu-id="d2866-112">500 kbps Peer-to-peer quality video calling 360p at 30fps</span></span>

- <span data-ttu-id="d2866-113">30 fpsで HD 720 p の解像度での 1.2 Mbps ピアツーピア HD 品質ビデオ通話</span><span class="sxs-lookup"><span data-stu-id="d2866-113">1.2 Mbps Peer-to-peer HD quality video calling with resolution of HD 720p at 30fps</span></span>

- <span data-ttu-id="d2866-114">30 fpsで HD 1080 p の解像度での 1.5 Mbps ピアツーピア HD 品質ビデオ通話</span><span class="sxs-lookup"><span data-stu-id="d2866-114">1.5 Mbps Peer-to-peer HD quality video calling with resolution of HD 1080p at 30fps</span></span>

- <span data-ttu-id="d2866-115">500 kbps / 1 Mbps のグループビデオ通話</span><span class="sxs-lookup"><span data-stu-id="d2866-115">500kbps/1Mbps Group Video calling</span></span>

- <span data-ttu-id="d2866-116">1Mbps/2Mbps の HD グループビデオ通話 (1080 p の画面で 540 p のビデオ) </span><span class="sxs-lookup"><span data-stu-id="d2866-116">1Mbps/2Mbps HD Group video calling (540p videos on 1080p screen)</span></span>

<span data-ttu-id="d2866-117">詳細については、「[Microsoft Teams 用に組織のネットワークを準備する](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d2866-117">For more information, see [Prepare your organization's network for Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span></span>
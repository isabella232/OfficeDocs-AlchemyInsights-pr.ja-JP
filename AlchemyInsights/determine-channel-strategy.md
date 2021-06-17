---
title: チャネル戦略を決定する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9144"
- "9005291"
- "11089"
- "9006490"
ms.openlocfilehash: c47218035155a8138caeac01e03fbe9d9e1aca4d
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989658"
---
# <a name="determine-channel-strategy"></a><span data-ttu-id="3c011-102">チャネル戦略を決定する</span><span class="sxs-lookup"><span data-stu-id="3c011-102">Determine channel strategy</span></span>

<span data-ttu-id="3c011-103">Microsoft Edge は、ブラウザーの更新頻度を制御する 4 つのチャネルでリリースされます。</span><span class="sxs-lookup"><span data-stu-id="3c011-103">Microsoft Edge is released in four channels that control how often the browser is updated.</span></span> <span data-ttu-id="3c011-104">各チャネルのより詳細な概要については、[チャネルの概要](/DeployEdge/microsoft-edge-channels#channel-overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c011-104">For a more in-depth overview of each channel, see [Channel overview](/DeployEdge/microsoft-edge-channels#channel-overview).</span></span>

<span data-ttu-id="3c011-105">[安定チャネル] は、ほとんどのデバイスに展開する必要があるチャネルですが、複数のチャネルとデバイスの展開を検討する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3c011-105">The Stable Channel is the one you'll want to deploy to most devices, but you should consider deploying multiple channels and devices.</span></span>

> [!NOTE]
> <span data-ttu-id="3c011-106">1 つのデバイスに複数のチャネルをインストールできます。</span><span class="sxs-lookup"><span data-stu-id="3c011-106">You can install more than one channel on a single device.</span></span>

<span data-ttu-id="3c011-107">**複数のデバイスとチャネル**</span><span class="sxs-lookup"><span data-stu-id="3c011-107">**Multiple devices and channels**</span></span>

<span data-ttu-id="3c011-108">ベータ チャネルまたはテスト チャネルを使用するようにデバイスのサブセットを構成することをお勧めします。これにより、組織全体に移動する前に、今後の変更を確認してテストできます。</span><span class="sxs-lookup"><span data-stu-id="3c011-108">We recommend having a subset of devices configured to use the beta or test channel, so that you can see upcoming changes and test them before they go to your whole organization.</span></span>

<span data-ttu-id="3c011-109">デバイスに複数のチャネルをインストールすると、問題が発生した場合にユーザーが安定したチャネルに簡単に切り替えることができるため、新しいバージョンをテストするリスクを減らすことができます。</span><span class="sxs-lookup"><span data-stu-id="3c011-109">Installing multiple channels on a device can reduce the risk of testing a new version, because the users can easily switch to the stable channel if they run into issues.</span></span>

<span data-ttu-id="3c011-110">チャネル戦略を定義したら、ポリシーの定義を開始する準備が整います。</span><span class="sxs-lookup"><span data-stu-id="3c011-110">Once you've defined your channel strategy, you're ready to start defining policies.</span></span>


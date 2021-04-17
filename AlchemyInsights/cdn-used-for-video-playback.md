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
# <a name="cdn-used-for-video-playback"></a>ビデオの再生に使用される CDN

Stream および外部アプリからのライブ イベントや、Yammer または Teams からのデバイス ライブ イベントには、自動的に Azure CDN が使用されます。 Stream にアップロードしたオンデマンドのビデオは、まだ、再生の際に Azure CDN が使用されません。 Stream のライブ以外のビデオは、テナントの地理的リージョン内でテナントに関連付けられた Azure Media Services 配信元サーバーから再生されます。 詳細については、次の記事を参照してください。

- [ビデオの再生に使用される CDN](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)

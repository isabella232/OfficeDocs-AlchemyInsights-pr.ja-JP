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
ms.openlocfilehash: 399be421994437d4cd2df644531334c58d177ec3293e7e379d84cd8326823a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54071121"
---
# <a name="cdn-used-for-video-playback"></a>ビデオの再生に使用される CDN

Stream および外部アプリからのライブ イベントや、Yammer または Teams からのデバイス ライブ イベントには、自動的に Azure CDN が使用されます。 Stream にアップロードしたオンデマンドのビデオは、まだ、再生の際に Azure CDN が使用されません。 Stream のライブ以外のビデオは、テナントの地理的リージョン内でテナントに関連付けられた Azure Media Services 配信元サーバーから再生されます。 詳細については、次の記事を参照してください。

- [ビデオの再生に使用される CDN](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)

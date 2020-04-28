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
# <a name="cdn-used-for-video-playback"></a>ビデオの再生に使用される CDN

Stream および外部アプリからのライブ イベントや、Yammer または Teams からのデバイス ライブ イベントには、自動的に Azure CDN が使用されます。 Stream にアップロードしたオンデマンドのビデオは、まだ、再生の際に Azure CDN が使用されません。 Stream のライブ以外のビデオは、テナントの地理的リージョン内でテナントに関連付けられた Azure Media Services 配信元サーバーから再生されます。 詳細については、次の記事を参照してください。

- [ビデオの再生に使用される CDN](https://docs.microsoft.com/ja-JP/stream/network-overview#cdn-used-for-video-playback)

---
title: ビデオの再生に使用される CDN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: 6bc87783375a206a84c96eb7ddd58db5bfd31728
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756972"
---
# <a name="cdn-used-for-video-playback"></a>ビデオの再生に使用される CDN

Stream および外部アプリからのライブ イベントや、Yammer または Teams からのデバイス ライブ イベントには、自動的に Azure CDN が使用されます。 Stream にアップロードしたオンデマンドのビデオは、まだ、再生の際に Azure CDN が使用されません。 Stream のライブ以外のビデオは、テナントの地理的リージョン内でテナントに関連付けられた Azure Media Services 配信元サーバーから再生されます。 詳細については、次の記事を参照してください。

- [ビデオの再生に使用される CDN](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)

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
ms.openlocfilehash: c40606df4a79fed1e526440f7f27f8f15dbd2032
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2020
ms.locfileid: "44058865"
---
# <a name="cdn-used-for-video-playback"></a>ビデオの再生に使用される CDN

Stream および外部アプリからのライブ イベントや、Yammer または Teams からのデバイス ライブ イベントには、自動的に Azure CDN が使用されます。 Stream にアップロードしたオンデマンドのビデオは、まだ、再生の際に Azure CDN が使用されません。 Stream のライブ以外のビデオは、テナントの地理的リージョン内でテナントに関連付けられた Azure Media Services 配信元サーバーから再生されます。 詳細については、次の記事を参照してください。

- [ビデオの再生に使用される CDN](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)

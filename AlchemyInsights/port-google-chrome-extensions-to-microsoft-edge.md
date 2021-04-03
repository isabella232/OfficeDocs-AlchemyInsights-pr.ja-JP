---
title: Google Chrome 拡張機能を Microsoft Edge (Chromium) に移植する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
- "8297"
- "9004617"
ms.openlocfilehash: 1c71d74d01c1e38e4c7789aea2c0b43701b3a5de
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505289"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Google Chrome 拡張機能を Microsoft Edge (Chromium) に移植する

簡単に [Google Chrome 拡張機能を Microsoft Edge (Chromium) に移植する](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)ことができます。 通常は、最小限の変更だけで、これらの拡張機能を Microsoft Edge で実行できます。

Google Chrome でサポートされている拡張機能 API とマニフェスト キーは、Microsoft Edge と互換性のあるコードです。 ただし、Microsoft Edge では拡張機能 API chrome.gcm、chrome.identity.getAccounts、chrome.identity.getAuthToken、chrome.instanceID はサポートされていません。
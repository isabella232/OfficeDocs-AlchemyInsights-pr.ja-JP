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
ms.openlocfilehash: 34ec7e71a2f27eb5b46395876a4d1c903189be1050e523796c9f2a817c20aaa0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973702"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Google Chrome 拡張機能を Microsoft Edge (Chromium) に移植する

簡単に [Google Chrome 拡張機能を Microsoft Edge (Chromium) に移植する](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)ことができます。 通常は、最小限の変更だけで、これらの拡張機能を Microsoft Edge で実行できます。

Google Chrome でサポートされている拡張機能 API とマニフェスト キーは、Microsoft Edge と互換性のあるコードです。 ただし、Microsoft Edge では拡張機能 API chrome.gcm、chrome.identity.getAccounts、chrome.identity.getAuthToken、chrome.instanceID はサポートされていません。
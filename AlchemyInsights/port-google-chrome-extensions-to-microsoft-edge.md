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
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2020
ms.locfileid: "49680464"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="937a0-102">Google Chrome 拡張機能を Microsoft Edge (Chromium) に移植する</span><span class="sxs-lookup"><span data-stu-id="937a0-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="937a0-103">簡単に [Google Chrome 拡張機能を Microsoft Edge (Chromium) に移植する](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)ことができます。</span><span class="sxs-lookup"><span data-stu-id="937a0-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="937a0-104">通常は、最小限の変更だけで、これらの拡張機能を Microsoft Edge で実行できます。</span><span class="sxs-lookup"><span data-stu-id="937a0-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="937a0-105">Google Chrome でサポートされている拡張機能 API とマニフェスト キーは、Microsoft Edge と互換性のあるコードです。</span><span class="sxs-lookup"><span data-stu-id="937a0-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="937a0-106">ただし、Microsoft Edge では拡張機能 API chrome.gcm、chrome.identity.getAccounts、chrome.identity.getAuthToken、chrome.instanceID はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="937a0-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>
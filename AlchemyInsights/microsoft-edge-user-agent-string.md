---
title: Microsoft Edge ユーザー エージェント文字列 (デスクトップ)
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
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/09/2020
ms.locfileid: "49680494"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="20af7-102">Microsoft Edge ユーザー エージェント文字列 (デスクトップ)</span><span class="sxs-lookup"><span data-stu-id="20af7-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="20af7-103">ユーザー エージェント (UA) の文字列を使用すると、特定のオペレーティング システムで使用されている特定のブラウザーのバージョンを検出できます。</span><span class="sxs-lookup"><span data-stu-id="20af7-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="20af7-104">他のブラウザーと同様に、Microsoft Edge はサイトに要求を行うたびに、この情報を「User-Agent」HTTP ヘッダーに含めます。</span><span class="sxs-lookup"><span data-stu-id="20af7-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="20af7-105">ブラウザーのバージョン情報には、「navigator.userAgent」の値を照会することによっても JavaScript 経由でアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="20af7-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="20af7-106">Web 開発者は、可能な限り機能の検出を使用して、コードの保守性を向上させ、コードの脆弱性を軽減し、将来の UA 文字列更新時にコードが破損するリスクを排除することを推奨します。</span><span class="sxs-lookup"><span data-stu-id="20af7-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="20af7-107">詳細については、「[Microsoft Edge ユーザー エージェント文字列 (デスクトップ)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20af7-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>
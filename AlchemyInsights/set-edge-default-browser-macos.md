---
title: Mac OS デバイスの既定ブラウザとして Microsoft Edge を設定する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/30/2021
ms.locfileid: "51492338"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="9d4fd-102">Mac OS デバイスの既定ブラウザとして Microsoft Edge を設定する</span><span class="sxs-lookup"><span data-stu-id="9d4fd-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="9d4fd-103">次の 2 つの方法のいずれかを使用して、Microsof tEdge を既定のブラウザーとして設定します。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="9d4fd-104">方法 1 : Microsoft Edge が既に既定のブラウザーとして設定されている macOS のイメージでデバイスをフラッシュします。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="9d4fd-105">方法 2 : DefaultBrowserSettingEnabled ポリシーを設定して、Microsoft Edge を既定のブラウザーとして設定するようにユーザーに促します。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="9d4fd-106">どちらの方法でも、ユーザーは既定のブラウザを変更できます。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="9d4fd-107">このため、メソッド 1 を使用した場合でも、DefaultBrowserSettingEnabled ポリシーを展開することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="9d4fd-108">ポリシーの展開後にユーザーが既定のブラウザーを変更すると、ポリシーにより、既定のブラウザーを Microsoft Edge に戻すようにユーザーに求められます。</span><span class="sxs-lookup"><span data-stu-id="9d4fd-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>

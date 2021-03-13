---
title: Windows 10 デバイスの Microsoft Defender Advanced Threat Protection へのオンボーディングに関する問題をリモートで修正する
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751374"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="71a1c-102">Windows 10 デバイスの Microsoft Defender Advanced Threat Protection へのオンボーディングに関する問題をリモートで修正する</span><span class="sxs-lookup"><span data-stu-id="71a1c-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="71a1c-103">リモート コンピューターにアクセスできる場合は、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="71a1c-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="71a1c-104">[クライアント接続アナライザー](https://go.microsoft.com/fwlink/?linkid=2143466)の診断ツールをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="71a1c-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="71a1c-105">展開し、MDATPAnalyzer.cmd を実行します。</span><span class="sxs-lookup"><span data-stu-id="71a1c-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="71a1c-106">MDATPClientAnalyzerResult フォルダーにある診断ログを見つけます。これは、アナライザー ツールがダウンロードされたフォルダーと同じです。</span><span class="sxs-lookup"><span data-stu-id="71a1c-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="71a1c-107">ログ ファイル MDATPClientAnalyzer.txt を確認して、接続またはインターネット プロキシ設定に関する問題を見つけます。</span><span class="sxs-lookup"><span data-stu-id="71a1c-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="71a1c-108">詳細については、「[マシンのオンボードの問題](https://go.microsoft.com/fwlink/?linkid=2143634)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71a1c-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>

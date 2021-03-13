---
title: Mac での MDATP インストールの問題を解決
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751353"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="f6b7a-102">Mac での MDATP インストールの問題を解決</span><span class="sxs-lookup"><span data-stu-id="f6b7a-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="f6b7a-103">手動によるインストールに失敗した場合、インストール ウィザードの **サマリー** ページでは次のエラーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="f6b7a-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="f6b7a-104">"インストール中にエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="f6b7a-104">"An error occurred during installation.</span></span> <span data-ttu-id="f6b7a-105">インストーラーでエラーが発生し、インストールに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="f6b7a-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="f6b7a-106">ソフトウェア製造元にお問い合わせください。"</span><span class="sxs-lookup"><span data-stu-id="f6b7a-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="f6b7a-107">MDM 展開では、このページに一般的なインストール エラーも表示されます。</span><span class="sxs-lookup"><span data-stu-id="f6b7a-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="f6b7a-108">エンド ユーザーに正確なエラーは表示されませんが、**/Library/Logs/Microsoft/mdatp/install.log** でインストールの進行状況に関するログ ファイルを保持しています。</span><span class="sxs-lookup"><span data-stu-id="f6b7a-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="f6b7a-109">このログ ファイルには、各インストール セッションが追加されます。</span><span class="sxs-lookup"><span data-stu-id="f6b7a-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="f6b7a-110">最後のインストール セッションのみを出力するには、`sed` を使用します。</span><span class="sxs-lookup"><span data-stu-id="f6b7a-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="f6b7a-111">詳細については、「[Mac 用 Microsoft Defender ATP のインストールの問題を解決](https://go.microsoft.com/fwlink/?linkid=2144615)」を参照します。</span><span class="sxs-lookup"><span data-stu-id="f6b7a-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>

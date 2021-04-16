---
title: ライセンス承認の問題 - 現在接続できない
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806447"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="2b0ac-102">Microsoft 365 アプリの「現在接続できません」メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="2b0ac-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="2b0ac-103">このメッセージが表示された場合は、次を試してください。</span><span class="sxs-lookup"><span data-stu-id="2b0ac-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="2b0ac-104">ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、インターネットが Microsoft 365 アプリにアクセスするのをそれらがブロックしていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="2b0ac-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="2b0ac-105">「[Microsoft の URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b0ac-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="2b0ac-106">[**開始**] > [**実行**] に移動して、**services.msc** と入力します。</span><span class="sxs-lookup"><span data-stu-id="2b0ac-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="2b0ac-107">次のサービスがすべて実行されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="2b0ac-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="2b0ac-108">ネットワーク接続デバイスの自動セットアップ</span><span class="sxs-lookup"><span data-stu-id="2b0ac-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="2b0ac-109">ネットワーク リスト サービス</span><span class="sxs-lookup"><span data-stu-id="2b0ac-109">Network List Service</span></span>
    - <span data-ttu-id="2b0ac-110">ネットワーク上の場所の認知</span><span class="sxs-lookup"><span data-stu-id="2b0ac-110">Network Location Awareness</span></span>
    - <span data-ttu-id="2b0ac-111">Windows イベント ログ</span><span class="sxs-lookup"><span data-stu-id="2b0ac-111">Windows Event Log</span></span>

<span data-ttu-id="2b0ac-112">これらのサービスのいずれかが実行されていない場合は、開始してみてください。</span><span class="sxs-lookup"><span data-stu-id="2b0ac-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="2b0ac-113">サービスの開始に問題がある場合は、昇格されたアクセス許可でコマンド プロンプトを開いて次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="2b0ac-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="2b0ac-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="2b0ac-114">**sfc /scannow**</span></span>

<span data-ttu-id="2b0ac-115">このコマンドが終了したら、コンピューターを再起動します。</span><span class="sxs-lookup"><span data-stu-id="2b0ac-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="2b0ac-116">詳細については、「[Microsoft 365 から Office のライセンス認証を行う際の "申し訳ありませんが、アカウントに接続できません。しばらくしてからもう一度お試しください"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)」エラーを参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b0ac-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>
---
title: ライセンス承認の問題 - 現在接続できない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716177"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="22e34-102">Office アプリの「現在接続できません」メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="22e34-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="22e34-103">このメッセージが表示された場合は、次を試してください。</span><span class="sxs-lookup"><span data-stu-id="22e34-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="22e34-104">ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、インターネットが Office アプリにアクセスするのをそれらがブロックしていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="22e34-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="22e34-105">「 [Microsoft url と IP アドレスの範囲」を](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)参照してください。</span><span class="sxs-lookup"><span data-stu-id="22e34-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="22e34-106">[**開始**] > [**実行**] に移動して、**services.msc** と入力します。</span><span class="sxs-lookup"><span data-stu-id="22e34-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="22e34-107">次のサービスがすべて実行されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="22e34-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="22e34-108">ネットワーク接続デバイスの自動セットアップ</span><span class="sxs-lookup"><span data-stu-id="22e34-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="22e34-109">ネットワーク リスト サービス</span><span class="sxs-lookup"><span data-stu-id="22e34-109">Network List Service</span></span>
    - <span data-ttu-id="22e34-110">ネットワーク上の場所の認知</span><span class="sxs-lookup"><span data-stu-id="22e34-110">Network Location Awareness</span></span>
    - <span data-ttu-id="22e34-111">Windows イベント ログ</span><span class="sxs-lookup"><span data-stu-id="22e34-111">Windows Event Log</span></span>

<span data-ttu-id="22e34-112">これらのサービスのいずれかが実行されていない場合は、開始してみてください。</span><span class="sxs-lookup"><span data-stu-id="22e34-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="22e34-113">サービスの開始に問題がある場合は、昇格されたアクセス許可でコマンド プロンプトを開いて次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="22e34-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="22e34-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="22e34-114">**sfc /scannow**</span></span>

<span data-ttu-id="22e34-115">このコマンドが終了したら、コンピューターを再起動します。</span><span class="sxs-lookup"><span data-stu-id="22e34-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="22e34-116">詳細については、「[申し訳ございません。アカウントに接続できません。」を参照してください。Microsoft 365 から Office をライセンス認証する際に、後でもう一度実行](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)してください。</span><span class="sxs-lookup"><span data-stu-id="22e34-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>
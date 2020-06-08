---
title: Microsoft 365 アプリの「申し訳ありませんが、一時的なサーバーの問題が発生しています」メッセージの修正
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582708"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="bb632-102">Microsoft 365 アプリの「申し訳ありませんが、一時的なサーバーの問題が発生しています」メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="bb632-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="bb632-103">このメッセージが表示された場合は、次を試してください。</span><span class="sxs-lookup"><span data-stu-id="bb632-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="bb632-104">ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、インターネットが Microsoft 365 アプリにアクセスするのをそれらがブロックしていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="bb632-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="bb632-105">「 [URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb632-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="bb632-106">[**開始**] > [**実行**] に移動して、**services.msc** と入力します。</span><span class="sxs-lookup"><span data-stu-id="bb632-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="bb632-107">次のサービスがすべて実行されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="bb632-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="bb632-108">ネットワーク接続デバイスの自動セットアップ</span><span class="sxs-lookup"><span data-stu-id="bb632-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="bb632-109">ネットワーク リスト サービス</span><span class="sxs-lookup"><span data-stu-id="bb632-109">Network List Service</span></span>
    - <span data-ttu-id="bb632-110">ネットワーク上の場所の認知</span><span class="sxs-lookup"><span data-stu-id="bb632-110">Network Location Awareness</span></span>
    - <span data-ttu-id="bb632-111">Windows イベント ログ</span><span class="sxs-lookup"><span data-stu-id="bb632-111">Windows Event Log</span></span>

<span data-ttu-id="bb632-112">これらのサービスのいずれかが実行されていない場合は、開始してみてください。</span><span class="sxs-lookup"><span data-stu-id="bb632-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="bb632-113">サービスの開始に問題がある場合は、昇格されたアクセス許可でコマンド プロンプトを開いて次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="bb632-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="bb632-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="bb632-114">**sfc /scannow**</span></span>

<span data-ttu-id="bb632-115">このコマンドが終了したら、コンピューターを再起動します。</span><span class="sxs-lookup"><span data-stu-id="bb632-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="bb632-116">詳細については、「[ライセンス認証を行う際の ”申し訳ありませんが、アカウントに接続できません。しばらくしてからもう一度お試しください”](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)」エラーを参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb632-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>
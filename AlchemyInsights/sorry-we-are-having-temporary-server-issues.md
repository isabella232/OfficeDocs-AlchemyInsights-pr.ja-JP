---
title: Office アプリを修正しています。一時的なサーバーの問題メッセージが表示されています。
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627995"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="cb768-102">Office アプリの「申し訳ありませんが、一時的なサーバーの問題が発生しています」メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="cb768-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="cb768-103">このメッセージが表示された場合は、次を試してください。</span><span class="sxs-lookup"><span data-stu-id="cb768-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="cb768-104">ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、インターネットが Office アプリにアクセスするのをそれらがブロックしていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="cb768-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="cb768-105">詳細については、「[Office 365 の URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb768-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="cb768-106">[**開始**] > [**実行**] に移動して、**services.msc** と入力します。</span><span class="sxs-lookup"><span data-stu-id="cb768-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="cb768-107">次のサービスがすべて実行されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="cb768-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="cb768-108">ネットワーク接続デバイスの自動セットアップ</span><span class="sxs-lookup"><span data-stu-id="cb768-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="cb768-109">ネットワーク リスト サービス</span><span class="sxs-lookup"><span data-stu-id="cb768-109">Network List Service</span></span>
    - <span data-ttu-id="cb768-110">ネットワーク上の場所の認知</span><span class="sxs-lookup"><span data-stu-id="cb768-110">Network Location Awareness</span></span>
    - <span data-ttu-id="cb768-111">Windows イベント ログ</span><span class="sxs-lookup"><span data-stu-id="cb768-111">Windows Event Log</span></span>

<span data-ttu-id="cb768-112">これらのサービスのいずれかが実行されていない場合は、開始してみてください。</span><span class="sxs-lookup"><span data-stu-id="cb768-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="cb768-113">サービスの開始に問題がある場合は、昇格されたアクセス許可でコマンド プロンプトを開いて次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="cb768-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="cb768-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="cb768-114">**sfc /scannow**</span></span>

<span data-ttu-id="cb768-115">このコマンドが終了したら、コンピューターを再起動します。</span><span class="sxs-lookup"><span data-stu-id="cb768-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="cb768-116">詳細については、「[Office 365 から Office のライセンス認証を行う際の ”申し訳ありませんが、アカウントに接続できません。しばらくしてからもう一度お試しください”](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)」エラーを参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb768-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>
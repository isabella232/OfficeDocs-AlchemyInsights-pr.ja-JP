---
title: OneDrive のエラー 0x8004de40 の修正
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755853"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="88c04-102">OneDrive のエラー 0x8004de40 の修正</span><span class="sxs-lookup"><span data-stu-id="88c04-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="88c04-103">OneDrive でエラー 0x8004de40 が発生した場合は、次の操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="88c04-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="88c04-104">Acitve ディレクトリ ドメインに接続されている間に、影響を受けたコンピューターを再起動します。</span><span class="sxs-lookup"><span data-stu-id="88c04-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="88c04-105">再起動で問題が修正しない場合は、Azure AD からデバイスを切断してから再度参加させます。</span><span class="sxs-lookup"><span data-stu-id="88c04-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="88c04-106">**注**: 次の手順を実行している間、社内ネットワーク上にいなければなりません。</span><span class="sxs-lookup"><span data-stu-id="88c04-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="88c04-107">例えば旅行中など、社内インフラストラクチャに接続できない場合は、これらの手順を実行しないでください。</span><span class="sxs-lookup"><span data-stu-id="88c04-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="88c04-108">管理者特権でコマンド プロンプトを開きます。</span><span class="sxs-lookup"><span data-stu-id="88c04-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="88c04-109">管理者特権でコマンド プロンプトを開くには、[**スタート**] をクリックし、[**コマンド プロンプト**] を右クリックして、[**管理者として実行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="88c04-109">To open an elevated Command Prompt window, click **Start**, point to All Programs, click Accessories, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="88c04-110">「*dsregcmd /leave*」と入力して**Enter**キーを押します。</span><span class="sxs-lookup"><span data-stu-id="88c04-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="88c04-111">操作が終了したら、「*dsregcmd /join*」と入力して**Enter**キーを押します。</span><span class="sxs-lookup"><span data-stu-id="88c04-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="88c04-112">完了したら、コマンド プロンプトを閉じます。</span><span class="sxs-lookup"><span data-stu-id="88c04-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="88c04-113">コンピューターを再起動して、OneDrive にログインします。</span><span class="sxs-lookup"><span data-stu-id="88c04-113">Reboot the computer, and log into OneDrive.</span></span>
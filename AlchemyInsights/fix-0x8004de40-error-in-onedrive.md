---
title: OneDrive での0x8004de40 エラーの修正
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525064"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="0958a-102">OneDrive での0x8004de40 エラーの修正</span><span class="sxs-lookup"><span data-stu-id="0958a-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="0958a-103">OneDrive を使用してエラーを受信した場合は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="0958a-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="0958a-104">Acitve Directory ドメインに接続している間に、影響を受けたコンピューターを再起動します。</span><span class="sxs-lookup"><span data-stu-id="0958a-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="0958a-105">再起動しても問題が解決されない場合は、Azure AD からデバイスを分離して再参加させてください。</span><span class="sxs-lookup"><span data-stu-id="0958a-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="0958a-106">**注**: これらの手順を実行している間は、企業ネットワークにログオンする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0958a-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="0958a-107">企業インフラストラクチャ (出張中など) に接続できない場合は、これらの手順を実行しないでください。</span><span class="sxs-lookup"><span data-stu-id="0958a-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="0958a-108">管理者特権でのコマンド プロンプトを開きます。</span><span class="sxs-lookup"><span data-stu-id="0958a-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="0958a-109">昇格したコマンドプロンプトを開くには、[**スタート**] をクリックし、[**コマンドプロンプト**] を右クリックし、[**管理者として実行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0958a-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="0958a-110">「 *Dsregcmd/Leave* 」と入力し、 **enter**キーを押します。</span><span class="sxs-lookup"><span data-stu-id="0958a-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="0958a-111">完了したら、「 *dsregcmd/join* 」と入力し、 **enter**キーを押します。</span><span class="sxs-lookup"><span data-stu-id="0958a-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="0958a-112">完了したら、コマンドプロンプトを閉じます。</span><span class="sxs-lookup"><span data-stu-id="0958a-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="0958a-113">コンピューターを再起動して、OneDrive にログインします。</span><span class="sxs-lookup"><span data-stu-id="0958a-113">Reboot the computer, and log into OneDrive.</span></span>
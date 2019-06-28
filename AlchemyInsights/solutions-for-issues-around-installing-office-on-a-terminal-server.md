---
title: ターミナル サーバーに Office をインストールするときの問題の解決方法
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: 6e877493f44b4636e1293582b5baf6bf98d1d251
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "32373717"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a><span data-ttu-id="a5566-102">ターミナル サーバーに Office をインストールするときの問題の解決方法</span><span class="sxs-lookup"><span data-stu-id="a5566-102">Solutions for issues around installing office on a Terminal Server</span></span>

<span data-ttu-id="a5566-103">共有コンピューターのライセンス認証を使用するには、Office 365 ProPlus が含まれている Office 365 プランを保有している必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5566-103">To use shared computer activation, you must have an Office 365 plan that includes Office 365 ProPlus.</span></span>
  
- <span data-ttu-id="a5566-104">共有コンピューターのライセンス認証が Office 365 ProPlus に対して有効になっていることを確認する</span><span class="sxs-lookup"><span data-stu-id="a5566-104">Verify that shared computer activation is enabled for Office 365 ProPlus</span></span>
    
- <span data-ttu-id="a5566-105">Office 365 ProPlus のライセンス認証が成功したことを確認する</span><span class="sxs-lookup"><span data-stu-id="a5566-105">Verify that activation for Office 365 ProPlus succeeded</span></span>
    
- <span data-ttu-id="a5566-106">共有コンピューターのライセンス認証に関する次のエラー メッセージを確認します。</span><span class="sxs-lookup"><span data-stu-id="a5566-106">Review error messages for shared computer activation:</span></span>
    
  - <span data-ttu-id="a5566-107">"お客様がアカウントにお持ちの製品では、共有コンピューター シナリオで Office をライセンス認証することができません。"</span><span class="sxs-lookup"><span data-stu-id="a5566-107">"The products we found in your account cannot be used to activate Office in shared computer scenarios"</span></span>
  
<span data-ttu-id="a5566-108">このエラーは、Office 365 ProPlus を含む Office 365 のプランがないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="a5566-108">This error means that you don't have an Office 365 plan that includes Office 365 ProPlus.</span></span>
    
  - <span data-ttu-id="a5566-109">"ライセンスのない製品"</span><span class="sxs-lookup"><span data-stu-id="a5566-109">"Unlicensed Product"</span></span>
    
  - <span data-ttu-id="a5566-110">ユーザーに Office 365 ProPlus のライセンスが割り当てられていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a5566-110">Check that the user is assigned a license for Office 365 ProPlus.</span></span>
    
  - <span data-ttu-id="a5566-111">ユーザーが Office 365 のユーザー アカウントでサインインしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a5566-111">Check that the user signs in with her user account for Office 365</span></span>
    
  - <span data-ttu-id="a5566-112">共有のコンピューターからインターネットに接続していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a5566-112">Check that there is connectivity between the shared computer and the Internet.</span></span>
    
<span data-ttu-id="a5566-113">その他のトラブルシューティング上のヒントについては、「[Office 365 ProPlus に対する共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5566-113">For other troubleshooting tips, please see: [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)</span></span>
  


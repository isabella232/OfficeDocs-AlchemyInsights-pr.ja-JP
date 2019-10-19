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
ms.openlocfilehash: bed91bf59219a19d5742d3ca4a61718c34b5c774
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/18/2019
ms.locfileid: "36501480"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a><span data-ttu-id="45099-102">ターミナル サーバーに Office をインストールするときの問題の解決方法</span><span class="sxs-lookup"><span data-stu-id="45099-102">Solutions for issues around installing office on a Terminal Server</span></span>

<span data-ttu-id="45099-103">共有コンピューターのライセンス認証を使用するには、Office 365 ProPlus が含まれている Office 365 プランを保有している必要があります。</span><span class="sxs-lookup"><span data-stu-id="45099-103">To use shared computer activation, you must have an Office 365 plan that includes Office 365 ProPlus.</span></span>
  
- <span data-ttu-id="45099-104">共有コンピューターのライセンス認証が Office 365 ProPlus に対して有効になっていることを確認する</span><span class="sxs-lookup"><span data-stu-id="45099-104">Verify that shared computer activation is enabled for Office 365 ProPlus</span></span>
    
- <span data-ttu-id="45099-105">Office 365 ProPlus のライセンス認証が成功したことを確認する</span><span class="sxs-lookup"><span data-stu-id="45099-105">Verify that activation for Office 365 ProPlus succeeded</span></span>
    
- <span data-ttu-id="45099-106">共有コンピューターのライセンス認証に関する次のエラー メッセージを確認します。</span><span class="sxs-lookup"><span data-stu-id="45099-106">Review error messages for shared computer activation:</span></span>
    
  - <span data-ttu-id="45099-107">"お客様がアカウントにお持ちの製品では、共有コンピューター シナリオで Office をライセンス認証することができません。"</span><span class="sxs-lookup"><span data-stu-id="45099-107">"The products we found in your account cannot be used to activate Office in shared computer scenarios"</span></span>
  
<span data-ttu-id="45099-108">このエラーは、Office 365 ProPlus を含む Office 365 のプランがないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="45099-108">This error means that you don't have an Office 365 plan that includes Office 365 ProPlus.</span></span>
    
  - <span data-ttu-id="45099-109">"ライセンスのない製品"</span><span class="sxs-lookup"><span data-stu-id="45099-109">"Unlicensed Product"</span></span>
    
  - <span data-ttu-id="45099-110">ユーザーに Office 365 ProPlus のライセンスが割り当てられていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="45099-110">Check that the user is assigned a license for Office 365 ProPlus.</span></span>
    
  - <span data-ttu-id="45099-111">ユーザーが Office 365 のユーザー アカウントでサインインしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="45099-111">Check that the user signs in with her user account for Office 365</span></span>
    
  - <span data-ttu-id="45099-112">共有のコンピューターからインターネットに接続していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="45099-112">Check that there is connectivity between the shared computer and the Internet.</span></span>
    
<span data-ttu-id="45099-113">その他のトラブルシューティング上のヒントについては、「[Office 365 ProPlus に対する共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45099-113">For other troubleshooting tips, please see: [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)</span></span>
  


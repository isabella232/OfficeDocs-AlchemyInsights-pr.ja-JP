---
title: ターミナル サーバーに Office をインストールするときの問題の解決方法
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: da69592fd0f55a4bfce45d271aeca5cde1f659b2
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43712679"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a><span data-ttu-id="f08f9-102">ターミナル サーバーに Office をインストールするときの問題の解決方法</span><span class="sxs-lookup"><span data-stu-id="f08f9-102">Solutions for issues around installing office on a Terminal Server</span></span>

<span data-ttu-id="f08f9-103">共有コンピューターのライセンス認証を使用するには、Microsoft 365 Apps for enterprise を含むサブスクリプションが必要です。</span><span class="sxs-lookup"><span data-stu-id="f08f9-103">To use shared computer activation, you must have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>
  
- <span data-ttu-id="f08f9-104">共有コンピューターのライセンス認証が有効になっていることを確認する</span><span class="sxs-lookup"><span data-stu-id="f08f9-104">Verify that shared computer activation is enabled</span></span>
- <span data-ttu-id="f08f9-105">ライセンス認証が正常に完了したことを確認する</span><span class="sxs-lookup"><span data-stu-id="f08f9-105">Verify that activation succeeded</span></span>
- <span data-ttu-id="f08f9-106">共有コンピューターのライセンス認証に関する次のエラー メッセージを確認します。</span><span class="sxs-lookup"><span data-stu-id="f08f9-106">Review error messages for shared computer activation:</span></span>
- <span data-ttu-id="f08f9-107">"お客様がアカウントにお持ちの製品では、共有コンピューター シナリオで Office をライセンス認証することができません。"</span><span class="sxs-lookup"><span data-stu-id="f08f9-107">"The products we found in your account cannot be used to activate Office in shared computer scenarios"</span></span>
  
<span data-ttu-id="f08f9-108">このエラーは、エンタープライズ向けの Microsoft 365 アプリを含むサブスクリプションがないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="f08f9-108">This error means that you don't have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>

<span data-ttu-id="f08f9-109">"ライセンスのない製品"</span><span class="sxs-lookup"><span data-stu-id="f08f9-109">"Unlicensed Product"</span></span>

- <span data-ttu-id="f08f9-110">ユーザーにエンタープライズ向け Microsoft 365 アプリのライセンスが割り当てられていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f08f9-110">Check that the user is assigned a license for Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="f08f9-111">ユーザーが自分のユーザーアカウントでサインインしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f08f9-111">Check that the user signs in with their user account.</span></span>
- <span data-ttu-id="f08f9-112">共有のコンピューターからインターネットに接続していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f08f9-112">Check that there is connectivity between the shared computer and the Internet.</span></span>

<span data-ttu-id="f08f9-113">他のトラブルシューティングのヒントについては、「[共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f08f9-113">For other troubleshooting tips, please see: [Troubleshoot issues with shared computer activation](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)</span></span>
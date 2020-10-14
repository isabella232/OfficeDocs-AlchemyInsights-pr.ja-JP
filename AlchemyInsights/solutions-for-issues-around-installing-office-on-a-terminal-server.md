---
title: ターミナル サーバーに Office をインストールするときの問題の解決方法
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: df1a50031196fbd79662cee620fc41c7be14e179
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47738462"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a><span data-ttu-id="e42d0-102">ターミナル サーバーに Office をインストールするときの問題の解決方法</span><span class="sxs-lookup"><span data-stu-id="e42d0-102">Solutions for issues around installing office on a Terminal Server</span></span>

<span data-ttu-id="e42d0-103">共有コンピューターのライセンス認証を使用するには、Microsoft 365 Apps for enterprises を含むサブスクリプションが必要です。</span><span class="sxs-lookup"><span data-stu-id="e42d0-103">To use shared computer activation, you must have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>
  
- <span data-ttu-id="e42d0-104">共有コンピューターのライセンス認証が有効になっていることを確認する</span><span class="sxs-lookup"><span data-stu-id="e42d0-104">Verify that shared computer activation is enabled</span></span>
- <span data-ttu-id="e42d0-105">ライセンス認証に成功したことを確認する</span><span class="sxs-lookup"><span data-stu-id="e42d0-105">Verify that activation succeeded</span></span>
- <span data-ttu-id="e42d0-106">共有コンピューターのライセンス認証に関する次のエラー メッセージを確認します。</span><span class="sxs-lookup"><span data-stu-id="e42d0-106">Review error messages for shared computer activation:</span></span>
- <span data-ttu-id="e42d0-107">"お客様がアカウントにお持ちの製品では、共有コンピューター シナリオで Office をライセンス認証することができません。"</span><span class="sxs-lookup"><span data-stu-id="e42d0-107">"The products we found in your account cannot be used to activate Office in shared computer scenarios"</span></span>
  
<span data-ttu-id="e42d0-108">このエラーは、Microsoft 365 Apps for enterprise を含むサブスクリプションがないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="e42d0-108">This error means that you don't have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>

<span data-ttu-id="e42d0-109">"ライセンスのない製品"</span><span class="sxs-lookup"><span data-stu-id="e42d0-109">"Unlicensed Product"</span></span>

- <span data-ttu-id="e42d0-110">ユーザーに Microsoft 365 Apps for enterprise のライセンスが割り当てられていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="e42d0-110">Check that the user is assigned a license for Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="e42d0-111">ユーザーがユーザー アカウントでサインインしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="e42d0-111">Check that the user signs in with their user account.</span></span>
- <span data-ttu-id="e42d0-112">共有のコンピューターからインターネットに接続していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="e42d0-112">Check that there is connectivity between the shared computer and the Internet.</span></span>

<span data-ttu-id="e42d0-113">その他のトラブルシューティング上のヒントについては、「[共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e42d0-113">For other troubleshooting tips, please see: [Troubleshoot issues with shared computer activation](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span></span>
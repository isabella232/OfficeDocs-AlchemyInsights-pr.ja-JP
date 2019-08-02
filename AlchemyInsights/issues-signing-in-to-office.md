---
title: Office アプリへのサインインの問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "36051955"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="7f453-102">Office アプリの空白のサインイン画面</span><span class="sxs-lookup"><span data-stu-id="7f453-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="7f453-103">この問題を解決するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="7f453-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="7f453-104">[Windows](https://support.microsoft.com/help/4027667/windows-10-update)および[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)の最新の更新プログラムをインストールします。</span><span class="sxs-lookup"><span data-stu-id="7f453-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="7f453-105">Internet explorer のオプションをリセットする: [**ツール** > ] [インターネット**オプション** > の詳細設定]**[** > **internet explorer の設定をリセット**する] (カスタム設定が失われることに注意してください)。その後、Office にもう一度サインインします。</span><span class="sxs-lookup"><span data-stu-id="7f453-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="7f453-106">Windows Defender Application Guard (WDAG) または同様のファイアウォールまたはウイルス対策プログラムを無効にします。</span><span class="sxs-lookup"><span data-stu-id="7f453-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="7f453-107">コントロールパネルで、[**プログラム**] に移動し、[ **Windows の機能の有効化または無効化**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7f453-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="7f453-108">Windows Defender Application Guard が有効になっている場合は、無効にしてみてください。</span><span class="sxs-lookup"><span data-stu-id="7f453-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="7f453-109">**注:** コンピューターの再起動が必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="7f453-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="7f453-110">Microsoft AAD プラグイン[AAD WAM プラグイン](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)が、アプリケーションまたはファイアウォール/ウイルス対策プログラムによってブロックされていないことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="7f453-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="7f453-111">Windows 資格情報マネージャーを使用して[Office 資格情報をクリア](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)します。</span><span class="sxs-lookup"><span data-stu-id="7f453-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="7f453-112">**注:** Office 2016 のレジストリパスは16.0 に変更されました。</span><span class="sxs-lookup"><span data-stu-id="7f453-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7f453-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="7f453-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="7f453-114">詳細については、「 [Windows 10 の Office 2016 ビルド16.0.7967 での更新後のサインインの接続の問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f453-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>
---
title: Windows 10 のスタートアップ設定
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2020
ms.locfileid: "42410592"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="f9771-102">Windows 10 のスタートアップ設定</span><span class="sxs-lookup"><span data-stu-id="f9771-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="f9771-103">**起動時に自動的に実行されるアプリを変更する**</span><span class="sxs-lookup"><span data-stu-id="f9771-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="f9771-104">[[設定] > アプリ > スタートアップ](ms-settings:startupapps?activationSource=GetHelp)] に移動します。</span><span class="sxs-lookup"><span data-stu-id="f9771-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="f9771-105">起動時に実行するアプリがオン**に**なっていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="f9771-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="f9771-106">**起動時に自動的に実行されるようにアプリを追加する**</span><span class="sxs-lookup"><span data-stu-id="f9771-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="f9771-107">[**スタート**] をクリックまたはタップして、起動時に実行するアプリを見つけます。</span><span class="sxs-lookup"><span data-stu-id="f9771-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="f9771-108">アプリを右クリックし、[**その他**] をクリックし、[**ファイルの場所を開く**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f9771-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="f9771-109">これにより、アプリのショートカットが保存される場所が開きます。</span><span class="sxs-lookup"><span data-stu-id="f9771-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="f9771-110">開いているファイルの場所を指定するオプションがない場合は、起動時にアプリを実行できないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="f9771-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="f9771-111">ファイルの場所を開いた状態で、 **Windows ロゴキー + R**を押し、「 **shell: startup**」と入力して、[ **OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f9771-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="f9771-112">これにより、スタートアップフォルダーが開きます。</span><span class="sxs-lookup"><span data-stu-id="f9771-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="f9771-113">ショートカットをコピーして、[ファイルの場所] から [Startup] フォルダーに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="f9771-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="f9771-114">**高度なスタートアップオプション (セーフモード、UEFI 設定、別のデバイスからのブートを含む)**</span><span class="sxs-lookup"><span data-stu-id="f9771-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="f9771-115">作業内容を保存し、開いているドキュメントをすべて閉じます。これらの手順は PC を再起動するためです。</span><span class="sxs-lookup"><span data-stu-id="f9771-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="f9771-116">[設定] に移動して[& セキュリティ > 回復 > 更新](ms-settings:recovery?activationSource=GetHelp)します。</span><span class="sxs-lookup"><span data-stu-id="f9771-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="f9771-117">[**詳細スタートアップ**] で、[**今すぐ再起動**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f9771-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="f9771-118">PC がオプションの選択画面に再起動したら、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="f9771-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="f9771-119">USB ドライブなどのデバイスからブートするには、[**デバイスを使用**する] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f9771-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="f9771-120">UEFI 設定 (BIOS セットアップとも呼ばれます) を入力するには、[**トラブルシューティング] [> Advanced options > UEFI ファームウェア設定**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f9771-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="f9771-121">セーフモードを入力するか、または [詳細なスタートアップ設定] を変更するには、[**トラブルシューティング > advanced options > Startup settings**] をクリックし、[**再起動**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f9771-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="f9771-122">[BitLocker 回復キー](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)の入力を求められる場合があります。</span><span class="sxs-lookup"><span data-stu-id="f9771-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="f9771-123">PC が再度再起動したら、使用するスタートアップ設定をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f9771-123">After your PC restarts again, click the startup setting you want to use.</span></span>
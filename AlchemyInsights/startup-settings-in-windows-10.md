---
title: Windows 10 の起動設定
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751140"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="80a1d-102">Windows 10 の起動設定</span><span class="sxs-lookup"><span data-stu-id="80a1d-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="80a1d-103">**起動時に自動的に実行されるアプリを変更する**</span><span class="sxs-lookup"><span data-stu-id="80a1d-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="80a1d-104">[[設定]、[アプリ]、[スタートアップ]](ms-settings:startupapps?activationSource=GetHelp) の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="80a1d-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="80a1d-105">起動時に実行するアプリが [**オン**] になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="80a1d-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="80a1d-106">**起動時に自動的に実行されるアプリを追加する**</span><span class="sxs-lookup"><span data-stu-id="80a1d-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="80a1d-107">[**スタート**] をクリックまたはタップし、起動時に実行するアプリを検索します。</span><span class="sxs-lookup"><span data-stu-id="80a1d-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="80a1d-108">アプリを右クリックし、[**詳細**]、[**ファイルの場所を開く**] の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="80a1d-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="80a1d-109">アプリのショートカットが保存されている場所が開きます。</span><span class="sxs-lookup"><span data-stu-id="80a1d-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="80a1d-110">[ファイルの場所を開く] というオプションが表示されない場合は、このアプリは起動時に実行することはできないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="80a1d-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="80a1d-111">ファイルの場所が開いた状態で、**Windows ロゴ + R キー**を押し、「**shell:startup**」と入力し、[**OK**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="80a1d-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="80a1d-112">[スタートアップ] フォルダーが開きます。</span><span class="sxs-lookup"><span data-stu-id="80a1d-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="80a1d-113">ファイルの場所からアプリのショートカットをコピーし、[スタートアップ] フォルダーに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="80a1d-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="80a1d-114">**起動の詳細オプション (セーフ モード、UEFI 設定、別のデバイスからのブートなど)**</span><span class="sxs-lookup"><span data-stu-id="80a1d-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="80a1d-115">次の手順では PC を再起動するため、作業を保存し、開かれているすべてのドキュメントを閉じます。</span><span class="sxs-lookup"><span data-stu-id="80a1d-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="80a1d-116">[[設定]、[更新とセキュリティ]、[回復]](ms-settings:recovery?activationSource=GetHelp) の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="80a1d-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="80a1d-117">[**PC の起動をカスタマイズする**] の下で、[**今すぐ再起動**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="80a1d-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="80a1d-118">PC が再起動して [オプションの選択] 画面が表示されたら、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="80a1d-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="80a1d-119">USB ドライブなどのデバイスから起動するには、[**デバイスの使用**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="80a1d-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="80a1d-120">UEFI 設定 (BIOS セットアップと呼ばれることもあります) を入力するには、**[トラブルシューティング ]、[詳細オプション]、[UEFI ファームウェアの設定]** の順にクリックします。 </span><span class="sxs-lookup"><span data-stu-id="80a1d-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="80a1d-121">セーフ モードで起動する場合、または起動の詳細設定を変更する場合は、**[トラブルシューティング]、[詳細オプション]、[スタートアップ設定]** の順にクリックし、[**再起動**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="80a1d-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="80a1d-122">[Bitlocker 回復キー](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)の入力を求めるメッセージが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="80a1d-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="80a1d-123">PC が再び再起動したら、使用する起動設定をクリックします。</span><span class="sxs-lookup"><span data-stu-id="80a1d-123">After your PC restarts again, click the startup setting you want to use.</span></span>
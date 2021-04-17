---
title: プリンターのトラブルシューティングを行う
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001214"
- "3186"
ms.openlocfilehash: 37bc4c1a8f39084e06b6f291c1245fa163e7b638
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830479"
---
# <a name="troubleshoot-your-printer"></a><span data-ttu-id="80c9a-102">プリンターのトラブルシューティングを行う</span><span class="sxs-lookup"><span data-stu-id="80c9a-102">Troubleshoot your printer</span></span>

<span data-ttu-id="80c9a-103">まず、**プリンター電源サイクル** を試します。</span><span class="sxs-lookup"><span data-stu-id="80c9a-103">First try a **printer power cycle**.</span></span> <span data-ttu-id="80c9a-104">次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="80c9a-104">Follow these steps:</span></span>

1. <span data-ttu-id="80c9a-105">プリンターをオフにし、電源ケーブルを取り外します。</span><span class="sxs-lookup"><span data-stu-id="80c9a-105">Turn off your printer and unplug its power cable.</span></span>

2. <span data-ttu-id="80c9a-106">30 秒間待ちます。</span><span class="sxs-lookup"><span data-stu-id="80c9a-106">Wait 30 seconds.</span></span>

3. <span data-ttu-id="80c9a-107">プリンターを電源に再接続し、再びオンにします。</span><span class="sxs-lookup"><span data-stu-id="80c9a-107">Plug your printer back in and turn the printer back on.</span></span>

<span data-ttu-id="80c9a-108">それでも問題が解決しない場合は、**[スタート] > [設定] > [更新とセキュリティ] > [トラブルシューティング]** の順に移動し、プリンターのトラブルシューティング ツールを実行します。</span><span class="sxs-lookup"><span data-stu-id="80c9a-108">If that did not solve your problem, run the Printer troubleshooter by going to **Start > Settings > Update & Security > Troubleshoot**.</span></span> <span data-ttu-id="80c9a-109">[**プリンター**] クリック、[**トラブルシューティング ツールの実行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="80c9a-109">Click **Printer**, and then click **Run the troubleshooter**.</span></span>

<span data-ttu-id="80c9a-110">**プリンターがネットワーク接続経由で PC に接続されている場合** (急いでいる場合は、USB ケーブルを使用してプリンターを PC に直接接続すると、プリンターをすばやく動作させることができます):</span><span class="sxs-lookup"><span data-stu-id="80c9a-110">**If your printer is connected to your PC via network connection** (if you're in a hurry, you may be able to get your printer working quickly by using a USB cable to plug your printer directly into your PC):</span></span>

1. <span data-ttu-id="80c9a-111">**プリンターのネットワーク接続を確認します**。</span><span class="sxs-lookup"><span data-stu-id="80c9a-111">**Check your printer's network connection**.</span></span>
    
    - <span data-ttu-id="80c9a-112">プリンターの指示に従ってネットワーク接続を確認します。</span><span class="sxs-lookup"><span data-stu-id="80c9a-112">Follow your printer's instructions to check the network connection.</span></span>

    - <span data-ttu-id="80c9a-113">プリンターがネットワークに接続されていない場合は、デバイスの指示に従ってネットワークに接続します。</span><span class="sxs-lookup"><span data-stu-id="80c9a-113">If your printer isn't connected to a network, follow your device's instructions to get connected to your network.</span></span>

2. <span data-ttu-id="80c9a-114">**PC のネットワーク接続をプリンターの接続と一致させます**。</span><span class="sxs-lookup"><span data-stu-id="80c9a-114">**Match your PC's network connection to your printer's connection**.</span></span>

    - <span data-ttu-id="80c9a-115">**[スタート] > [設定] > [ネットワークとインターネット]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="80c9a-115">Click **Start > Settings > Network & Internet**.</span></span>

    - <span data-ttu-id="80c9a-116">[**ネットワークの状態**] の下で、ネットワーク名を検索します。</span><span class="sxs-lookup"><span data-stu-id="80c9a-116">Under **Networking status**, find your network name.</span></span> <span data-ttu-id="80c9a-117">これは、プリンターの接続名と完全に一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="80c9a-117">This needs to exactly match the printer's connection name.</span></span>

    - <span data-ttu-id="80c9a-118">これら 2 つの接続が異なる場合は、プリンターのネットワークに合わせて PC の接続を変更します。</span><span class="sxs-lookup"><span data-stu-id="80c9a-118">If these two connections are not the same, change your PC's connection to match the printer's network.</span></span>

<span data-ttu-id="80c9a-119">また、**ネットワーク プリンターを削除して再インストールする** こともできます。</span><span class="sxs-lookup"><span data-stu-id="80c9a-119">You may also try **removing and reinstalling your network printer**:</span></span>

1. <span data-ttu-id="80c9a-120">**[設定] でプリンターを削除します**。</span><span class="sxs-lookup"><span data-stu-id="80c9a-120">**Remove the printer in Settings**.</span></span>

    - <span data-ttu-id="80c9a-121">**[スタート] > [設定] > [デバイス] > [プリンターとスキャナー]** の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="80c9a-121">Click **Start > Settings > Devices > Printers & scanners**.</span></span>

    - <span data-ttu-id="80c9a-122">[プリンターとスキャナー] ヘッダーで、トラブルシューティングを行うプリンターをクリックします。</span><span class="sxs-lookup"><span data-stu-id="80c9a-122">Under the Printers & scanners header, click the printer you are troubleshooting.</span></span> <span data-ttu-id="80c9a-123">**[デバイスの削除]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="80c9a-123">Click **Remove device**.</span></span> <span data-ttu-id="80c9a-124">指示に従い、プリンターを完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="80c9a-124">Follow the instructions to fully remove the printer.</span></span>

2. <span data-ttu-id="80c9a-125">**サードパーティのプリンター製造元のソフトウェアを削除します**。</span><span class="sxs-lookup"><span data-stu-id="80c9a-125">**Remove any 3rd party printer manufacturer software**.</span></span>

    - <span data-ttu-id="80c9a-126">**[スタート] > [設定] > [アプリ]** の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="80c9a-126">Click **Start > Settings > Apps**.</span></span>

    - <span data-ttu-id="80c9a-127">[アプリと機能] ヘッダーで、スクロールし、プリンターの製造元 (HP、Canon、Epson など) によりインストールされたソフトウェアを見つけます。</span><span class="sxs-lookup"><span data-stu-id="80c9a-127">Under the Apps & features header, scroll to find any software installed from your printer's manufacturer (such as HP, Canon, or Epson).</span></span>

    - <span data-ttu-id="80c9a-128">ソフトウェアをクリックし、**[アンインストール]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="80c9a-128">Click the software and click **Uninstall**.</span></span>

3. <span data-ttu-id="80c9a-129">**プリンターをオフにして再起動します**。</span><span class="sxs-lookup"><span data-stu-id="80c9a-129">**Turn off and restart your printer**.</span></span>

    - <span data-ttu-id="80c9a-130">プリンターをオフにし、電源ケーブルを取り外します。</span><span class="sxs-lookup"><span data-stu-id="80c9a-130">Turn off your printer and unplug its power cable.</span></span> <span data-ttu-id="80c9a-131">30 秒間待ちます。</span><span class="sxs-lookup"><span data-stu-id="80c9a-131">Wait 30 seconds.</span></span> <span data-ttu-id="80c9a-132">プリンターを電源に再接続し、再びオンにします。</span><span class="sxs-lookup"><span data-stu-id="80c9a-132">Plug your printer back in and turn the printer back on.</span></span>

4. <span data-ttu-id="80c9a-133">**[設定] でプリンターを再インストールします**。</span><span class="sxs-lookup"><span data-stu-id="80c9a-133">**Reinstall your printer in Settings**.</span></span>

    - <span data-ttu-id="80c9a-134">**[スタート] > [設定] > [デバイス] > [プリンターとスキャナー]** の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="80c9a-134">Click **Start > Settings > Devices> Printers & scanners**.</span></span>
 
    - <span data-ttu-id="80c9a-135">画面の上部にある [**プリンターまたはスキャナーの追加**] をクリックし、指示に従ってプリンターを再インストールします。</span><span class="sxs-lookup"><span data-stu-id="80c9a-135">Click **Add printer or scanner** at the top of the screen and follow the instructions to reinstall your printer.</span></span>

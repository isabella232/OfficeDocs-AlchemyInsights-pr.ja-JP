---
title: 既存のモニターのトラブルシューティング
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690716"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="721e0-102">既存のモニターをトラブルシューティングする</span><span class="sxs-lookup"><span data-stu-id="721e0-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="721e0-103">モニターをトラブルシューティングするには、次の解決方法をお試しください。</span><span class="sxs-lookup"><span data-stu-id="721e0-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="721e0-104">**モニターの表示を更新する:**</span><span class="sxs-lookup"><span data-stu-id="721e0-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="721e0-105">Windows キー、Ctrl、Shift、B キーを同時に押します。これにより、グラフィック ドライバーとの通信が更新されます。</span><span class="sxs-lookup"><span data-stu-id="721e0-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="721e0-106">モニターが一瞬点滅し、数秒後に再び表示されます。</span><span class="sxs-lookup"><span data-stu-id="721e0-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="721e0-107">**モニター ハードウェアをトラブルシューティングする:**</span><span class="sxs-lookup"><span data-stu-id="721e0-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="721e0-108">PC とモニターを接続するケーブルを一旦抜いてから、再び差し込みます。</span><span class="sxs-lookup"><span data-stu-id="721e0-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="721e0-109">不必要なデバイス (アダプターやドックなど) をすべて PC から取り外します。</span><span class="sxs-lookup"><span data-stu-id="721e0-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="721e0-110">**更新プログラムを PC に最近インストールした場合は、ディスプレイ ドライバーを元に戻すことができます。**</span><span class="sxs-lookup"><span data-stu-id="721e0-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="721e0-111">[**スタート**] を選択し、"**デバイス マネージャー**" と入力し、表示される結果から [**デバイス マネージャー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="721e0-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="721e0-112">[**ディスプレイ アダプター**] セクションを展開し、使用しているディスプレイ アダプターを右クリックし、[**プロパティ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="721e0-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="721e0-113">[**ドライバー**] タブに移動し、[**ドライバーを元に戻す**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="721e0-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="721e0-114">注: このオプションが表示されない場合、または淡色表示されている場合は、下部にある [**キャンセル**] を選択し、次の手順に移ります。</span><span class="sxs-lookup"><span data-stu-id="721e0-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="721e0-115">これらの変更を反映させるには、PC の再起動が必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="721e0-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="721e0-116">**ディスプレイ ドライバーをアンインストールして再インストールする:**</span><span class="sxs-lookup"><span data-stu-id="721e0-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="721e0-117">[**スタート**] を選択し、"**デバイス マネージャー**" と入力し、表示される結果から [**デバイス マネージャー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="721e0-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="721e0-118">[**ディスプレイ アダプター**] セクションを展開し、使用しているディスプレイ アダプターを右クリックし、[**デバイスのアンインストール**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="721e0-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="721e0-119">[**このデバイスのドライバー ソフトウェアを削除します**] の横にあるチェック ボックスをオンにし、[**アンインストール**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="721e0-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="721e0-120">注: この段階でコンピューターの再起動を求められる場合があります。</span><span class="sxs-lookup"><span data-stu-id="721e0-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="721e0-121">再起動する前に、残りの手順を書き留めておいてください。</span><span class="sxs-lookup"><span data-stu-id="721e0-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="721e0-122">デバイス マネージャーをもう一度開きます。</span><span class="sxs-lookup"><span data-stu-id="721e0-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="721e0-123">[**ディスプレイ アダプター**] セクションを展開し、使用しているディスプレイ アダプターを右クリックし、[**ドライバーの更新**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="721e0-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="721e0-124">[**ドライバー ソフトウェアの最新版を自動検索します**] を選択し、インストールの手順に従います。</span><span class="sxs-lookup"><span data-stu-id="721e0-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>
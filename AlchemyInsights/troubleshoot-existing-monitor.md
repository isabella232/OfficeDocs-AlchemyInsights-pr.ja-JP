---
title: 既存のモニターのトラブルシューティング
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2019
ms.locfileid: "40791267"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="b51d4-102">既存のモニターのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="b51d4-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="b51d4-103">これらのソリューションを試して、モニターのトラブルシューティングを行います。</span><span class="sxs-lookup"><span data-stu-id="b51d4-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="b51d4-104">**モニターのディスプレイを更新します。**</span><span class="sxs-lookup"><span data-stu-id="b51d4-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="b51d4-105">次のキーを同時に押します。 Windows キー + Ctrl + Shift + B。これにより、グラフィックスドライバーとの通信が更新されます。</span><span class="sxs-lookup"><span data-stu-id="b51d4-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="b51d4-106">モニターは瞬間的に点滅し、数秒間で戻ります。</span><span class="sxs-lookup"><span data-stu-id="b51d4-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="b51d4-107">**モニターハードウェアのトラブルシューティング:**</span><span class="sxs-lookup"><span data-stu-id="b51d4-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="b51d4-108">PC をモニターに接続しているケーブルを外し、再度接続します。</span><span class="sxs-lookup"><span data-stu-id="b51d4-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="b51d4-109">PC (アダプターやドックなど) から重要ではないデバイスをすべて切断します。</span><span class="sxs-lookup"><span data-stu-id="b51d4-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="b51d4-110">**最近、PC に更新プログラムをインストールした場合は、ディスプレイドライバーをロールバックすることができます。**</span><span class="sxs-lookup"><span data-stu-id="b51d4-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="b51d4-111">[**スタート**] を選択し、「 **device manager**」と入力して、結果から [**デバイスマネージャー** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b51d4-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="b51d4-112">[**ディスプレイアダプター** ] セクションを展開し、ディスプレイアダプターを右クリックして [**プロパティ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b51d4-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="b51d4-113">[**ドライバー** ] タブに移動し、[**ドライバーのロールバック**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b51d4-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="b51d4-114">メモ: これが使用できないか、または淡色表示になっている場合は、次の手順に進むには、次のオプションから [**いいえ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b51d4-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="b51d4-115">これらの変更を有効にするには、PC を再起動する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="b51d4-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="b51d4-116">**ディスプレイドライバーをアンインストールして再インストールします。**</span><span class="sxs-lookup"><span data-stu-id="b51d4-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="b51d4-117">[**スタート**] を選択し、「 **device manager**」と入力して、結果から [**デバイスマネージャー** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b51d4-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="b51d4-118">[**ディスプレイアダプター** ] セクションを展開し、ディスプレイアダプターを右クリックし、[**アンインストールデバイス**の選択] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b51d4-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="b51d4-119">[**このデバイスのドライバーソフトウェアを削除**する] の横のボックスを選択し、[**アンインストール**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b51d4-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="b51d4-120">注: この段階で、コンピューターの再起動を求めるメッセージが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="b51d4-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="b51d4-121">再起動する前に、残りの手順を必ず書き留めておいてください。</span><span class="sxs-lookup"><span data-stu-id="b51d4-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="b51d4-122">デバイスマネージャーを再度開きます。</span><span class="sxs-lookup"><span data-stu-id="b51d4-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="b51d4-123">[**ディスプレイアダプター** ] セクションを展開し、ディスプレイアダプターを右クリックして、[**ドライバーの更新**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b51d4-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="b51d4-124">[**ドライバーソフトウェアを自動的に検索する**] を選択し、インストールの指示に従います。</span><span class="sxs-lookup"><span data-stu-id="b51d4-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>
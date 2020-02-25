---
title: Windows 10 のオーディオに関する問題をトラブルシューティングする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: f51fd233db5ae068e719f1cf3bc94a0dac82444f
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265021"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="5cc63-102">Windows 10 での音声の問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="5cc63-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="5cc63-103">**オーディオ トラブルシューティング ツールを実行する**</span><span class="sxs-lookup"><span data-stu-id="5cc63-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="5cc63-104">[[トラブルシューティング] 設定](ms-settings:troubleshoot)を開きます。</span><span class="sxs-lookup"><span data-stu-id="5cc63-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="5cc63-105">[**オーディオの再生**] > [**トラブルシューティング ツールの実行**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="5cc63-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="5cc63-106">**既定のデバイスを設定する**</span><span class="sxs-lookup"><span data-stu-id="5cc63-106">**Set the default device**</span></span>

<span data-ttu-id="5cc63-107">USB または HDMI を使用してオーディオ デバイスに接続している場合、そのデバイスを既定として設定する必要があることがあります。</span><span class="sxs-lookup"><span data-stu-id="5cc63-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="5cc63-108">**Start** > **sound**を開き、結果の一覧から [**サウンド**] または [**システムサウンドの変更**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="5cc63-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="5cc63-109">[**再生**] タブでデバイスを 1 つ選択し、[**既定値に設定**] を選択し、[**OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="5cc63-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="5cc63-110">**ケーブル、音量、スピーカー、およびヘッドフォンを確認する**</span><span class="sxs-lookup"><span data-stu-id="5cc63-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="5cc63-111">スピーカーとヘッドフォンの接続を確認してケーブルの緩みがないことを確かめ、ケーブルが正しいジャックに接続されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="5cc63-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="5cc63-112">電源と音量のレベルを確認して、すべてのボリュームコントロールをオンにしてみてください。</span><span class="sxs-lookup"><span data-stu-id="5cc63-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="5cc63-113">一部のスピーカーとアプリには独自のボリュームコントロールがあります。それらをすべて確認して、それらが正しいレベルであることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="5cc63-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="5cc63-114">別の USB ポートを使って接続してみます。</span><span class="sxs-lookup"><span data-stu-id="5cc63-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="5cc63-115">**注**: ヘッドフォンが接続されていると、スピーカーが動作しない場合があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="5cc63-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="5cc63-116">**デバイス マネージャーを確認する**</span><span class="sxs-lookup"><span data-stu-id="5cc63-116">**Check Device Manager**</span></span>

<span data-ttu-id="5cc63-117">ドライバーが最新であることをご確認するには、つぎの手順を実行してください。</span><span class="sxs-lookup"><span data-stu-id="5cc63-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="5cc63-118">[**スタート**] を選択し、"**デバイス マネージャー**" と入力し始め、表示される結果から [**デバイス マネージャー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="5cc63-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="5cc63-119">使用しているサウンド カードを [**サウンド、ビデオ、およびゲーム コントローラー**]で選択して開き、[**ドライバー**] タブを選択し、[**ドライバーの更新**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="5cc63-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="5cc63-120">**注**: Windows で新しいドライバーが見つからない場合は、デバイスの製造元の web サイトで新しいドライバーを探して、指示に従ってください。</span><span class="sxs-lookup"><span data-stu-id="5cc63-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="5cc63-121">**ドライバーを再インストールする**</span><span class="sxs-lookup"><span data-stu-id="5cc63-121">**Reinstall the driver**</span></span>

<span data-ttu-id="5cc63-122">デバイス　マネージャーで更新できない場合、または製造元の Web サイトで新しいドライバーを検索する場合は、次の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="5cc63-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="5cc63-123">デバイス マネージャーで、オーディ オ ドライバーを右クリック (または長押し) し、[**アンインストール**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="5cc63-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="5cc63-124">デバイスを再起動すると、Windows によりドライバーの再インストールが試みられます。</span><span class="sxs-lookup"><span data-stu-id="5cc63-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="5cc63-125">ドライバーの再インストールがうまくいかない場合は、Windows 付属の汎用オーディオ ドライバーを使用してみてください。</span><span class="sxs-lookup"><span data-stu-id="5cc63-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="5cc63-126">[デバイス マネージャー] を開き、使用しているオーディオ ドライバーを右クリック (または長押し) し、[**ドライバーの更新**] > [**コンピューターを参照してドライバー ソフトウェアを検索**] > [**コンピューター上の利用可能なドライバーの一覧から選択します**] の順に選択し、[**High Definition Audio デバイス**] を選択して [**次へ**] を選択し、指示に従ってインストールします。</span><span class="sxs-lookup"><span data-stu-id="5cc63-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

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
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/19/2019
ms.locfileid: "40825891"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a><span data-ttu-id="d29ba-102">Windows 10 のオーディオに関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="d29ba-102">Troubleshooting audio problems in Windows 10</span></span>

<span data-ttu-id="d29ba-103">**オーディオ トラブルシューティング ツールを実行する**</span><span class="sxs-lookup"><span data-stu-id="d29ba-103">**Run the audio troubleshooter**</span></span>

<span data-ttu-id="d29ba-104">オーディオ トラブルシューティング ツールを使用すると、オーディオの問題を自動的に修正できる場合があります。</span><span class="sxs-lookup"><span data-stu-id="d29ba-104">The audio troubleshooter might be able to fix the audio problems automatically:</span></span> 

1. <span data-ttu-id="d29ba-105">[**スタート**] を選択し、"**トラブルシューティング**" と入力し、結果の一覧から [**トラブルシューティング**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d29ba-105">Select **Start**, type **troubleshoot**, and then select **Troubleshoot** from the list of results.</span></span> 
2. <span data-ttu-id="d29ba-106">[**オーディオの再生**] > [**トラブルシューティング ツールの実行**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="d29ba-106">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="d29ba-107">**ケーブル、音量、スピーカー、およびヘッドフォンを確認する**</span><span class="sxs-lookup"><span data-stu-id="d29ba-107">**Check cables, volume, speakers, and headphones**</span></span>

- <span data-ttu-id="d29ba-108">スピーカーとヘッドフォンの接続を確認してケーブルの緩みがないことを確かめ、ケーブルが正しいジャックに接続されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="d29ba-108">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>
- <span data-ttu-id="d29ba-109">電源と音量レベルを確認し、すべての音量コントロールを上げてみます。</span><span class="sxs-lookup"><span data-stu-id="d29ba-109">Check your power and volume levels, and try turning all the volume controls up.</span></span>
- <span data-ttu-id="d29ba-110">一部のスピーカーおよびアプリには専用のボリューム コントロールがあるため、それらのコントロールをすべて確認しえ、正しいレベルで再生されていることを確認することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d29ba-110">Some speakers and apps have their own volume controls, and you might have to check them all to make sure they're at the right levels.</span></span>
- <span data-ttu-id="d29ba-111">別の USB ポートを使って接続してみます。</span><span class="sxs-lookup"><span data-stu-id="d29ba-111">Try connecting using a different USB port.</span></span>
- <span data-ttu-id="d29ba-112">**注:** ヘッドフォンが接続されているとスピーカーが機能しない場合があるので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="d29ba-112">**Note:** Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="d29ba-113">**デバイス マネージャーを確認する**</span><span class="sxs-lookup"><span data-stu-id="d29ba-113">**Check Device Manager**</span></span>

<span data-ttu-id="d29ba-114">ドライバーが最新であることをご確認するには、つぎの手順を実行してください。</span><span class="sxs-lookup"><span data-stu-id="d29ba-114">To make sure the drivers are up to date:</span></span>

- <span data-ttu-id="d29ba-115">[**スタート**] を選択し、"**デバイス マネージャー**" と入力し始め、表示される結果から [**デバイス マネージャー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d29ba-115">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="d29ba-116">使用しているサウンド カードを [**サウンド、ビデオ、およびゲーム コントローラー**]で選択して開き、[**ドライバー**] タブを選択し、[**ドライバーの更新**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d29ba-116">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span> 

<span data-ttu-id="d29ba-117">**注:** Windows で新しいドライバーが見つからない場合は、デバイスの製造元の Web サイトで新しいドライバーを検索し、インストール手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="d29ba-117">**Note:** If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="d29ba-118">**ドライバーを再インストールする**</span><span class="sxs-lookup"><span data-stu-id="d29ba-118">**Reinstall the driver**</span></span>

<span data-ttu-id="d29ba-119">デバイス　マネージャーで更新できない場合、または製造元の Web サイトで新しいドライバーを検索する場合は、次の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="d29ba-119">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span> 

1. <span data-ttu-id="d29ba-120">デバイス マネージャーで、オーディ オ ドライバーを右クリック (または長押し) し、[**アンインストール**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d29ba-120">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="d29ba-121">デバイスを再起動すると、Windows によりドライバーの再インストールが試みられます。</span><span class="sxs-lookup"><span data-stu-id="d29ba-121">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="d29ba-122">ドライバーの再インストールがうまくいかない場合は、Windows 付属の汎用オーディオ ドライバーを使用してみてください。</span><span class="sxs-lookup"><span data-stu-id="d29ba-122">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="d29ba-123">[デバイス マネージャー] を開き、使用しているオーディオ ドライバーを右クリック (または長押し) し、[**ドライバーの更新**] > [**コンピューターを参照してドライバー ソフトウェアを検索**] > [**コンピューター上の利用可能なドライバーの一覧から選択します**] の順に選択し、[**High Definition Audio デバイス**] を選択して [**次へ**] を選択し、指示に従ってインストールします。</span><span class="sxs-lookup"><span data-stu-id="d29ba-123">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

<span data-ttu-id="d29ba-124">**既定のデバイスを設定する**</span><span class="sxs-lookup"><span data-stu-id="d29ba-124">**Set the default device**</span></span>

<span data-ttu-id="d29ba-125">USB または HDMI を使用してオーディオ デバイスに接続している場合、そのデバイスを既定として設定する必要があることがあります。</span><span class="sxs-lookup"><span data-stu-id="d29ba-125">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span> 

1. <span data-ttu-id="d29ba-126">[**スタート**] を選択し "**サウンド**" と入力し、[**サウンド**] または [**システムが出す音の変更**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d29ba-126">Select **Start**, type **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2. <span data-ttu-id="d29ba-127">[**再生**] タブでデバイスを 1 つ選択し、[**既定値に設定**] を選択し、[**OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d29ba-127">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>


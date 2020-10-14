---
title: Windows 10 のオーディオに関する問題をトラブルシューティングする
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750313"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="19a68-102">Windows 10 のオーディオに関する問題をトラブルシューティングする</span><span class="sxs-lookup"><span data-stu-id="19a68-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="19a68-103">**オーディオ トラブルシューティング ツールを実行する**</span><span class="sxs-lookup"><span data-stu-id="19a68-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="19a68-104">[トラブルシューティングの設定](ms-settings:troubleshoot)を開きます。</span><span class="sxs-lookup"><span data-stu-id="19a68-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="19a68-105">[**オーディオの再生**] > [**トラブルシューティング ツールの実行**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="19a68-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="19a68-106">**既定のデバイスを設定する**</span><span class="sxs-lookup"><span data-stu-id="19a68-106">**Set the default device**</span></span>

<span data-ttu-id="19a68-107">USB または HDMI を使用してオーディオ デバイスに接続している場合、そのデバイスを既定として設定する必要があることがあります。</span><span class="sxs-lookup"><span data-stu-id="19a68-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="19a68-108">[**スタート**]  >  [**サウンド**] の順に開き、結果リストから [**サウンド**] または [**システムが出す音の変更**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="19a68-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="19a68-109">[**再生**] タブでデバイスを 1 つ選択し、[**既定値に設定**] を選択し、[**OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="19a68-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="19a68-110">**ケーブル、音量、スピーカー、およびヘッドフォンを確認する**</span><span class="sxs-lookup"><span data-stu-id="19a68-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="19a68-111">スピーカーとヘッドフォンの接続を確認してケーブルの緩みがないことを確かめ、ケーブルが正しいジャックに接続されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="19a68-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="19a68-112">電源と音量レベルを確認し、すべての音量コントロールを上げてみます。</span><span class="sxs-lookup"><span data-stu-id="19a68-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="19a68-113">一部のスピーカーおよびアプリには専用のボリューム コントロールがあるため、それらのコントロールをすべて確認しえ、正しいレベルで再生されていることを確認することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="19a68-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="19a68-114">別の USB ポートを使って接続してみます。</span><span class="sxs-lookup"><span data-stu-id="19a68-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="19a68-115">**注**: ヘッドフォンが接続されているとスピーカーが機能しない場合があるので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="19a68-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="19a68-116">**デバイス マネージャーを確認する**</span><span class="sxs-lookup"><span data-stu-id="19a68-116">**Check Device Manager**</span></span>

<span data-ttu-id="19a68-117">ドライバーが最新であることをご確認するには、つぎの手順を実行してください。</span><span class="sxs-lookup"><span data-stu-id="19a68-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="19a68-118">[**スタート**] を選択し、"**デバイス マネージャー**" と入力し始め、表示される結果から [**デバイス マネージャー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="19a68-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="19a68-119">使用しているサウンド カードを [**サウンド、ビデオ、およびゲーム コントローラー**]で選択して開き、[**ドライバー**] タブを選択し、[**ドライバーの更新**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="19a68-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="19a68-120">**注**: Windows で新しいドライバーが見つからない場合は、デバイスの製造元の Web サイトで新しいドライバーを検索し、インストール手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="19a68-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="19a68-121">**ドライバーを再インストールする**</span><span class="sxs-lookup"><span data-stu-id="19a68-121">**Reinstall the driver**</span></span>

<span data-ttu-id="19a68-122">デバイス　マネージャーで更新できない場合、または製造元の Web サイトで新しいドライバーを検索する場合は、次の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="19a68-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="19a68-123">デバイス マネージャーで、オーディ オ ドライバーを右クリック (または長押し) し、[**アンインストール**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="19a68-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="19a68-124">デバイスを再起動すると、Windows によりドライバーの再インストールが試みられます。</span><span class="sxs-lookup"><span data-stu-id="19a68-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="19a68-125">ドライバーの再インストールがうまくいかない場合は、Windows 付属の汎用オーディオ ドライバーを使用してみてください。</span><span class="sxs-lookup"><span data-stu-id="19a68-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="19a68-126">[デバイス マネージャー] を開き、使用しているオーディオ ドライバーを右クリック (または長押し) し、[**ドライバーの更新**] > [**コンピューターを参照してドライバー ソフトウェアを検索**] > [**コンピューター上の利用可能なドライバーの一覧から選択します**] の順に選択し、[**High Definition Audio デバイス**] を選択して [**次へ**] を選択し、指示に従ってインストールします。</span><span class="sxs-lookup"><span data-stu-id="19a68-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

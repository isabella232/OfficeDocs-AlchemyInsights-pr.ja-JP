---
title: Windows 10 で Bluetooth の問題を修正する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268959"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="3b4a4-102">Windows 10 で Bluetooth の問題を修正する</span><span class="sxs-lookup"><span data-stu-id="3b4a4-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="3b4a4-103">Bluetooth アイコンが不足しているか、Bluetooth のオンとオフを切り替えることができない場合は、Bluetooth のトラブルシューティングツールを実行することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="3b4a4-104">[[トラブルシューティング] 設定を開き](ms-settings:troubleshoot)、[**その他の問題を検出して修正**する] の下にある [ **Bluetooth** ] をクリックし、[**トラブルシューティングツールを実行する**</span><span class="sxs-lookup"><span data-stu-id="3b4a4-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="3b4a4-105">Bluetooth アイコンが表示されていない場合、Bluetooth はデバイスマネージャーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="3b4a4-106">デバイスマネージャーで、[ **Bluetooth**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="3b4a4-107">Bluetooth アダプター名を押したままにして (または右クリック) し、[**デバイスのアンインストール**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="3b4a4-108">Windows デバイスをシャットダウンし、数秒間待機してから、再度オンにします。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="3b4a4-109">Windows はドライバーの再インストールを試行します。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="3b4a4-110">最近 Windows 10 の更新プログラムをインストールしたか、Windows 10 にアップグレードした場合は、ドライバーの更新プログラムを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="3b4a4-111">デバイスマネージャーで、[ **bluetooth**] をクリックし、bluetooth アダプター名をクリックします ("radio" という単語が含まれている場合があります)。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="3b4a4-112">Bluetooth アダプターを押したままにして (または右クリックし) \*\*\*\* > 、**更新されたドライバーソフトウェアに対して [ドライバー検索を自動的に更新する**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="3b4a4-113">手順に従い、[**閉じる**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="3b4a4-114">Windows が新しい Bluetooth ドライバーを見つけられない場合は、PC の製造元の web サイトにアクセスして、そこから最新の Bluetooth ドライバーをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="3b4a4-115">ダウンロードしたら、[ドライバーの**更新** > ] をクリックし**てドライバーソフトウェア** > を参照し、ドライバーファイルが格納されている場所を**参照**し > **[OK]** > をクリックします。**次**に、インストールする手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="3b4a4-116">更新されたドライバーをインストールした後、コンピューターを再起動して、接続の問題が修正されていないかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="3b4a4-117">Bluetooth の問題のトラブルシューティング方法の詳細については、完全な記事「 [Windows 10 で bluetooth の問題を修正](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b4a4-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>

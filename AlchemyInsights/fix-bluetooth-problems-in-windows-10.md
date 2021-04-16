---
title: Windows 10 の Bluetooth の問題を解決する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812937"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="9205f-102">Windows 10 の Bluetooth の問題を解決する</span><span class="sxs-lookup"><span data-stu-id="9205f-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="9205f-103">Bluetooth アイコンが表示されない場合、または Bluetooth のオン/オフを切り替えることができない場合は、Bluetooth のトラブルシューティング ツールを実行します。</span><span class="sxs-lookup"><span data-stu-id="9205f-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="9205f-104">[[トラブルシューティングの設定] を開き](ms-settings:troubleshoot)、**[その他の問題の検出と解決]** にある **Bluetooth** をクリックして、**[トラブルシューティング ツールの実行]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9205f-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="9205f-105">Bluetooth アイコンは表示されないものの、デバイス マネージャーに Bluetooth が表示されている場合:</span><span class="sxs-lookup"><span data-stu-id="9205f-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="9205f-106">デバイス マネージャーで、**[Bluetooth]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9205f-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="9205f-107">Bluetooth アダプター名を長押し (または右クリック) し、**[デバイスのアンインストール]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9205f-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="9205f-108">Windows デバイスをシャットダウンし、数秒待ってから、再びオンにします。</span><span class="sxs-lookup"><span data-stu-id="9205f-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="9205f-109">Windows によりドライバーの再インストールが試みられます。</span><span class="sxs-lookup"><span data-stu-id="9205f-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="9205f-110">最近 Windows 10 の更新プログラムをインストールするか Windows 10 にアップグレードした場合は、ドライバーの更新プログラムを確認することができます。</span><span class="sxs-lookup"><span data-stu-id="9205f-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="9205f-111">デバイス マネージャーで、**[Bluetooth]** をクリックしてから、Bluetooth アダプター名 (radio という語が含まれている場合があります) をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9205f-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="9205f-112">Bluetooth アダプターを長押し (または右クリック) して、**[ドライバーの更新]** > **[ドライバー ソフトウェアの最新版を自動検索]** の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="9205f-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="9205f-113">手順に従って、**[閉じる]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9205f-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="9205f-114">Windows で新しい Bluetooth ドライバーが見つからない場合は、PC の製造元の Web サイトにアクセスし、そこから最新の Bluetooth ドライバーをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="9205f-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="9205f-115">ダウンロードしたら、**[ドライバーの更新]** > **[コンピューターを参照してドライバー ソフトウェアを検索]** > **[参照]** の順にクリックして、ドライバー ファイルが保存されている場所を選択し、**[OK]** > **[次へ]** の順に選択して、手順に従ってインストールします。</span><span class="sxs-lookup"><span data-stu-id="9205f-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="9205f-116">更新されたドライバーのインストールが完了したら、コンピューターを再起動し、接続の問題が解決されているか確認します。</span><span class="sxs-lookup"><span data-stu-id="9205f-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="9205f-117">Bluetooth の問題のトラブルシューティング方法の詳細については、「[Windows 10 の Bluetooth の問題を解決する](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)」と題する記事全体を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9205f-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>

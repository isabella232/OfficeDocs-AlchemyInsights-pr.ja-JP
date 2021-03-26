---
title: Windows 10 のドライブ領域を解放する
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038339"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="79d83-102">Windows 10 のドライブ領域を解放する</span><span class="sxs-lookup"><span data-stu-id="79d83-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="79d83-103">Windows のドライブ領域を解放するには、次の 2 つのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="79d83-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="79d83-104">Windows 10 のドライブ領域を解放します。</span><span class="sxs-lookup"><span data-stu-id="79d83-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="79d83-105">外部ストレージ デバイスを使って、Windows 10 更新プログラム用の領域を解放します。</span><span class="sxs-lookup"><span data-stu-id="79d83-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="79d83-106">ディスク クリーンアップを使用した後もディスク容量が少ない場合は、Temp フォルダーが、Microsoft Store で使用するアプリケーション (.appx) ファイルですぐにいっぱいになっている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="79d83-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="79d83-107">この問題を解決するには、Microsoft Store をリセットし、Microsoft Store のキャッシュをクリアして、Windows Update のトラブルシューティング ツールを実行します。</span><span class="sxs-lookup"><span data-stu-id="79d83-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="79d83-108">次の手順を実行する前に、Microsoft Store を閉じていることをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="79d83-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="79d83-109">**手順 1: Microsoft Store をリセットする**</span><span class="sxs-lookup"><span data-stu-id="79d83-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="79d83-110">**注** 設定やサインインの詳細など、デバイス上のアプリ データが完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="79d83-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="79d83-111">**[開始]** > **[設定]** > **[アプリ]** > **[アプリと機能]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="79d83-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="79d83-112">アプリの一覧で、Microsoft Store を見つけて選択します。</span><span class="sxs-lookup"><span data-stu-id="79d83-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="79d83-113">**[詳細オプション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="79d83-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="79d83-114">下にスクロールし、**[リセット]**、**[リセットの確認]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="79d83-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="79d83-115">**手順 2: Microsoft Store のキャッシュをクリアする**</span><span class="sxs-lookup"><span data-stu-id="79d83-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="79d83-116">Windows ロゴ キーを押しながら R キーを押して、[ファイル名を指定して実行] ダイアログ ボックスを開きます。</span><span class="sxs-lookup"><span data-stu-id="79d83-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="79d83-117">wsreset.exe と入力し、**[OK]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="79d83-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="79d83-118">空のコマンド プロンプト ウィンドウが開きます。</span><span class="sxs-lookup"><span data-stu-id="79d83-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="79d83-119">約 10 秒後に、ウィンドウが閉じて、Microsoft Store が自動的に開きます。</span><span class="sxs-lookup"><span data-stu-id="79d83-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="79d83-120">**手順 3: Windows Update をリセットする**</span><span class="sxs-lookup"><span data-stu-id="79d83-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="79d83-121">**[開始]** > **[設定]** > **[更新とセキュリティ]** > **[トラブルシューティング]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="79d83-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="79d83-122">下にスクロールし、一覧から **[Windows Update]** を選択し、**[トラブルシューティング ツールを実行する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="79d83-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="79d83-123">コンピューターを再起動し、問題が引き続き発生するかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="79d83-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>


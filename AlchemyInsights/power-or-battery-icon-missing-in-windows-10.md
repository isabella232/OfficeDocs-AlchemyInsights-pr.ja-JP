---
title: Windows 10 で電源アイコンまたはバッテリー アイコンが表示されない
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
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790553"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="d7f15-102">Windows 10 で電源アイコンまたはバッテリー アイコンが表示されない</span><span class="sxs-lookup"><span data-stu-id="d7f15-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="d7f15-103">Windows 10 デバイスにバッテリーが搭載されている場合 (たとえば、ノート PC またはタブレット、または USB 経由で UPS に接続された PC)、通常、電源/バッテリー アイコンが時計の近くのタスクバーに表示されます。次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="d7f15-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![バッテリー アイコン](media/battery-icon.png)

<span data-ttu-id="d7f15-105">このアイコンが表示されない場合は、非表示になっている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d7f15-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="d7f15-106">**[[設定]、[個人用設定]、[タスクバー]](ms-settings:taskbar?activationSource=GetHelp)** の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="d7f15-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="d7f15-107">通知領域で [**タスク バーに表示するアイコンの選択**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d7f15-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="d7f15-108">次に、リストから [**電源**] アイテムを見つけ、その設定を [**オン**] に切り替えます。</span><span class="sxs-lookup"><span data-stu-id="d7f15-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![タスクバーに電源アイコンを表示する](media/power-icon-on.png)

<span data-ttu-id="d7f15-110">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="d7f15-110">**Troubleshooting**</span></span>

<span data-ttu-id="d7f15-111">上記の手順に従っても、[**電源**] トグルが灰色表示されている、または表示されない場合は、タスクバーの検索ボックスに「**デバイス マネージャー**」と入力し、入力結果のリストから [**デバイス マネージャー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7f15-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="d7f15-112">[**バッテリー**] で、デバイスのバッテリーを右クリックし、[**無効にする**] をクリックして、[**はい**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d7f15-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="d7f15-113">数秒待ってからバッテリーを右クリックし、[**有効にする**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d7f15-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="d7f15-114">デバイスを再起動します。</span><span class="sxs-lookup"><span data-stu-id="d7f15-114">Then restart your device.</span></span>

<span data-ttu-id="d7f15-115">上記の手順に従っても、バッテリー アイコンがタスクバーに表示されない場合は、タスクバーの検索ボックスに「**デバイス マネージャー**」と入力し、入力結果のリストから [**デバイス マネージャー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7f15-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="d7f15-116">[**プロセス**] タブの [**名前**] で、[**エクスプローラー**] を右クリックし、[**再起動**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d7f15-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>

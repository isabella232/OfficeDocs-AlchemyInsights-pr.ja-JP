---
title: Windows 仮想デスクトップに Office と OneDrive をインストールする
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596095"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="e3c64-102">Windows 仮想デスクトップに Office と OneDrive をインストールする</span><span class="sxs-lookup"><span data-stu-id="e3c64-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="e3c64-103">[マスター VHD イメージを準備してカスタマイズします](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)。</span><span class="sxs-lookup"><span data-stu-id="e3c64-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="e3c64-104">仮想マシン (VM) がまだ作成されていない場合には、仮想マシンを作成します。</span><span class="sxs-lookup"><span data-stu-id="e3c64-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="e3c64-105">[共有コンピューターのライセンス認証モードで Office をインストールします](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)。</span><span class="sxs-lookup"><span data-stu-id="e3c64-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="e3c64-106">共有コンピューターのライセンス認証により、複数のユーザーが Office にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e3c64-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="e3c64-107">[マシンごとモードで OneDrive をインストールします](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)。</span><span class="sxs-lookup"><span data-stu-id="e3c64-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="e3c64-108">通常、OneDrive はユーザーごとにインストールされますが、ここではマシンごとにインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3c64-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>
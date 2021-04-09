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
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Windows 仮想デスクトップに Office と OneDrive をインストールする

1. [マスター VHD イメージを準備してカスタマイズします](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)。 仮想マシン (VM) がまだ作成されていない場合には、仮想マシンを作成します。

1. [共有コンピューターのライセンス認証モードで Office をインストールします](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)。 共有コンピューターのライセンス認証により、複数のユーザーが Office にアクセスできます。

1. [マシンごとモードで OneDrive をインストールします](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)。 通常、OneDrive はユーザーごとにインストールされますが、ここではマシンごとにインストールする必要があります。
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
ms.openlocfilehash: 226bd24a955f6165969102c8cf00cf45da537ee05a5363c74f1dfd055d922e1d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028621"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Windows 仮想デスクトップに Office と OneDrive をインストールする

1. [マスター VHD イメージを準備してカスタマイズします](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)。 仮想マシン (VM) がまだ作成されていない場合には、仮想マシンを作成します。

1. [共有コンピューターのライセンス認証モードで Office をインストールします](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)。 共有コンピューターのライセンス認証により、複数のユーザーが Office にアクセスできます。

1. [マシンごとモードで OneDrive をインストールします](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)。通常、OneDrive はユーザーごとにインストールされますが、ここではマシンごとにインストールする必要があります。
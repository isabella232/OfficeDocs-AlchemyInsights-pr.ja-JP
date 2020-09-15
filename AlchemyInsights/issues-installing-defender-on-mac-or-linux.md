---
title: Mac または Linux への Microsoft Defender のインストールに関する問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695491"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Mac または Linux への Microsoft Defender のインストールに関する問題

** Mac **

- Microsoft Defender ATP for Mac をインストールする前に、システム要件が満たされていることを確認してください。 詳細については、[「Microsoft Defender ATP for Macのインストール方法」](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)をご覧ください。  
- ファイル内の情報を確認します。「/Library/Logs/Microsoft/mdatp/install.log」。

** Linux **

- Linux 用の Microsoft Defender ATP をインストールする前に、システム要件が満たされていることを確認してください。 詳しくは、[「Microsoft Defender ATP for Linuxのインストール方法」](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)をご覧ください。 
- MDATPサービスが実行されていることを確認するには、[「インストールに失敗しました」](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)をご覧ください。  
    サービスが実行されていない場合の問題のトラブルシューティングと解決については、[「mdatpサービスが実行されていない場合のトラブルシューティングの手順」](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)をご覧ください。
- 製品の正常性を検証するクライアント構成を確認し、EICAR テキストファイルで検出テストを実行する手順については、[「クライアント構成」](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)をご覧ください。  

    **注**オンアクセスアクティビティでサポートされているファイルシステムのリストについては、[ 「Microsoft Defender ATP for Linux」 ](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)をご覧ください。
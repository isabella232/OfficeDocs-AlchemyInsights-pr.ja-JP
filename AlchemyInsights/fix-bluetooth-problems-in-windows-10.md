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
ms.openlocfilehash: 784f8c4d58bb8965cec2ce0a3722d0f16e36b16f914b4a154d6f6da58af9dc28
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53913900"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a>Windows 10 の Bluetooth の問題を解決する

Bluetooth アイコンが表示されない場合、または Bluetooth のオン/オフを切り替えることができない場合は、Bluetooth のトラブルシューティング ツールを実行します。 [[トラブルシューティングの設定] を開き](ms-settings:troubleshoot)、**[その他の問題の検出と解決]** にある **Bluetooth** をクリックして、**[トラブルシューティング ツールの実行]** をクリックします。

Bluetooth アイコンは表示されないものの、デバイス マネージャーに Bluetooth が表示されている場合:

1. デバイス マネージャーで、**[Bluetooth]** をクリックします。 Bluetooth アダプター名を長押し (または右クリック) し、**[デバイスのアンインストール]** をクリックします。

2. Windows デバイスをシャットダウンし、数秒待ってから、再びオンにします。Windows によりドライバーの再インストールが試みられます。

最近 Windows 10 の更新プログラムをインストールするか Windows 10 にアップグレードした場合は、ドライバーの更新プログラムを確認することができます。

1. デバイス マネージャーで、**[Bluetooth]** をクリックしてから、Bluetooth アダプター名 (radio という語が含まれている場合があります) をクリックします。

2. Bluetooth アダプターを長押し (または右クリック) して、**[ドライバーの更新]** > **[ドライバー ソフトウェアの最新版を自動検索]** の順にクリックします。 手順に従って、**[閉じる]** をクリックします。

      - Windows で新しい Bluetooth ドライバーが見つからない場合は、PC の製造元の Web サイトにアクセスし、そこから最新の Bluetooth ドライバーをダウンロードします。

    - ダウンロードしたら、**[ドライバーの更新]** > **[コンピューターを参照してドライバー ソフトウェアを検索]** > **[参照]** の順にクリックして、ドライバー ファイルが保存されている場所を選択し、**[OK]** > **[次へ]** の順に選択して、手順に従ってインストールします。

3. 更新されたドライバーのインストールが完了したら、コンピューターを再起動し、接続の問題が解決されているか確認します。

Bluetooth の問題のトラブルシューティング方法の詳細については、「[Windows 10 の Bluetooth の問題を解決する](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)」と題する記事全体を参照してください。

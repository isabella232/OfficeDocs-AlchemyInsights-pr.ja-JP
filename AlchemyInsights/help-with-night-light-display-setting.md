---
title: 夜間モードの表示設定を支援する
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
- "9005578"
- "9930"
ms.openlocfilehash: 7da8d4cefe2140340892544d73b9f8e3f3fdc679e9d58f2ad5ac12bf30830c5c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54078729"
---
# <a name="help-with-the-night-light-display-setting"></a>夜間モードの表示設定を支援する

夜間ディスプレイ設定の詳細については、「[Windows 10 でディスプレイを夜間用に設定する](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)」を参照してください。

[設定] で夜間モードのオプションがグレー表示されている場合は、ディスプレイ ドライバを確認してください。 

1. タスク バーの検索ボックスに「**デバイス マネージャー**」と入力し、検索結果のリストから [**デバイス マネージャー**] を選択します。
1. [**ディスプレイ アダプタ**] を展開します。 

残念ながら、デバイスが DisplayLink ドライバーまたは Basic Display ドライバーを使用している場合、夜間モード機能は使用できません。

夜間モード機能は最新のグラフィック テクノロジーを利用しているため、ディスプレイ ドライバーを更新する必要がある場合があります。  

- **[スタート]** > **[設定]** > **[更新とセキュリティ]** > **[Windows Update]** > **[更新の確認]** に移動して、更新を確認します。  

または

- ハードウェア メーカーのサポート Web サイトにアクセスして、最新のディスプレイ ドライバーを手動でダウンロードしてインストールします。

## <a name="reset-night-light-in-the-registry"></a>レジストリの夜間モードをリセットする

ディスプレイ ドライバの更新が機能しなかった場合は、レジストリの夜間モードをリセットする必要があるかもしれません。  

**注意:** このトラブルシューティング手順は、上級ユーザーにのみお勧めします。 レジストリを誤って変更すると、重大な問題が発生する可能性があります。 保護を強化するには、レジストリを変更する前にバックアップして、問題が発生した場合にレジストリを復元できるようにします。

1. 検索ボックスに「**regedit**」と入力し、検索結果で [**レジストリ エディタ**] を選択します。

1. 次のレジストリ キーに移動します。 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. 次のサブキーをエクスポートしてから削除します: $$windows.data.bluelightreduction.bluelightreductionstate

1. 次のサブキーをエクスポートしてから削除します：$$windows.data.bluelightreduction.settings

1. Windows を再起動し、常夜灯のオプションが利用可能かどうかを確認します。



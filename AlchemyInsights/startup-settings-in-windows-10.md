---
title: Windows 10 のスタートアップ設定
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2020
ms.locfileid: "42410592"
---
# <a name="startup-settings-in-windows-10"></a>Windows 10 のスタートアップ設定

**起動時に自動的に実行されるアプリを変更する**

1. [[設定] > アプリ > スタートアップ](ms-settings:startupapps?activationSource=GetHelp)] に移動します。

2. 起動時に実行するアプリがオン**に**なっていることを確認してください。

**起動時に自動的に実行されるようにアプリを追加する**

1. [**スタート**] をクリックまたはタップして、起動時に実行するアプリを見つけます。

2. アプリを右クリックし、[**その他**] をクリックし、[**ファイルの場所を開く**] をクリックします。 これにより、アプリのショートカットが保存される場所が開きます。 開いているファイルの場所を指定するオプションがない場合は、起動時にアプリを実行できないことを意味します。

3. ファイルの場所を開いた状態で、 **Windows ロゴキー + R**を押し、「 **shell: startup**」と入力して、[ **OK]** をクリックします。 これにより、スタートアップフォルダーが開きます。

4. ショートカットをコピーして、[ファイルの場所] から [Startup] フォルダーに貼り付けます。

**高度なスタートアップオプション (セーフモード、UEFI 設定、別のデバイスからのブートを含む)**

1. 作業内容を保存し、開いているドキュメントをすべて閉じます。これらの手順は PC を再起動するためです。

2. [設定] に移動して[& セキュリティ > 回復 > 更新](ms-settings:recovery?activationSource=GetHelp)します。

3. [**詳細スタートアップ**] で、[**今すぐ再起動**] をクリックします。 

4. PC がオプションの選択画面に再起動したら、次のようにします。

    - USB ドライブなどのデバイスからブートするには、[**デバイスを使用**する] をクリックします。

    - UEFI 設定 (BIOS セットアップとも呼ばれます) を入力するには、[**トラブルシューティング] [> Advanced options > UEFI ファームウェア設定**] をクリックします。 

    - セーフモードを入力するか、または [詳細なスタートアップ設定] を変更するには、[**トラブルシューティング > advanced options > Startup settings**] をクリックし、[**再起動**] をクリックします。 [BitLocker 回復キー](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)の入力を求められる場合があります。 PC が再度再起動したら、使用するスタートアップ設定をクリックします。
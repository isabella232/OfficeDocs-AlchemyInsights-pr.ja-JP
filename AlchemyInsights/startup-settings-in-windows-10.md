---
title: Windows 10 の起動設定
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828157"
---
# <a name="startup-settings-in-windows-10"></a>Windows 10 の起動設定

**起動時に自動的に実行されるアプリを変更する**

1. [[設定]、[アプリ]、[スタートアップ]](ms-settings:startupapps?activationSource=GetHelp) の順に移動します。

2. 起動時に実行するアプリが [**オン**] になっていることを確認します。

**起動時に自動的に実行されるアプリを追加する**

1. [**スタート**] をクリックまたはタップし、起動時に実行するアプリを検索します。

2. アプリを右クリックし、[**詳細**]、[**ファイルの場所を開く**] の順にクリックします。 アプリのショートカットが保存されている場所が開きます。 [ファイルの場所を開く] というオプションが表示されない場合は、このアプリは起動時に実行することはできないことを意味します。

3. ファイルの場所が開いた状態で、**Windows ロゴ + R キー** を押し、「**shell:startup**」と入力し、[**OK**] をクリックします。 [スタートアップ] フォルダーが開きます。

4. ファイルの場所からアプリのショートカットをコピーし、[スタートアップ] フォルダーに貼り付けます。

**起動の詳細オプション (セーフ モード、UEFI 設定、別のデバイスからのブートなど)**

1. 次の手順では PC を再起動するため、作業を保存し、開かれているすべてのドキュメントを閉じます。

2. [[設定]、[更新とセキュリティ]、[回復]](ms-settings:recovery?activationSource=GetHelp) の順に移動します。

3. [**PC の起動をカスタマイズする**] の下で、[**今すぐ再起動**] をクリックします。 

4. PC が再起動して [オプションの選択] 画面が表示されたら、次の操作を行います。

    - USB ドライブなどのデバイスから起動するには、[**デバイスの使用**] をクリックします。

    - UEFI 設定 (BIOS セットアップと呼ばれることもあります) を入力するには、**[トラブルシューティング ]、[詳細オプション]、[UEFI ファームウェアの設定]** の順にクリックします。  

    - セーフ モードで起動する場合、または起動の詳細設定を変更する場合は、**[トラブルシューティング]、[詳細オプション]、[スタートアップ設定]** の順にクリックし、[**再起動**] をクリックします。 [Bitlocker 回復キー](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)の入力を求めるメッセージが表示されることがあります。 PC が再び再起動したら、使用する起動設定をクリックします。
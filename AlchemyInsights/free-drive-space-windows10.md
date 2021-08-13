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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: c7d29ab718be8dbdcde61a7de2f158fb3bbd722d2964d8b13cde9936dd1e5ee1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928086"
---
# <a name="free-up-drive-space-in-windows-10"></a>Windows 10 のドライブ領域を解放する

Windows のドライブ領域を解放するには、次の 2 つのオプションがあります。

- Windows 10 のドライブ領域を解放します。
- 外部ストレージ デバイスを使って、Windows 10 更新プログラム用の領域を解放します。

ディスク クリーンアップを使用した後もディスク容量が少ない場合は、Temp フォルダーが、Microsoft Store で使用するアプリケーション (.appx) ファイルですぐにいっぱいになっている可能性があります。 この問題を解決するには、Microsoft Store をリセットし、Microsoft Store のキャッシュをクリアして、Windows Update のトラブルシューティング ツールを実行します。 次の手順を実行する前に、Microsoft Store を閉じていることをご確認ください。

**手順 1: Microsoft Store をリセットする**

**注** 設定やサインインの詳細など、デバイス上のアプリ データが完全に削除されます。

1. **[開始]** > **[設定]** > **[アプリ]** > **[アプリと機能]** を選択します。

1. アプリの一覧で、Microsoft Store を見つけて選択します。

1. **[詳細オプション]** を選択します。

1. 下にスクロールし、**[リセット]**、**[リセットの確認]** の順に選択します。

**手順 2: Microsoft Store のキャッシュをクリアする**

1. Windows ロゴ キーを押しながら R キーを押して、[ファイル名を指定して実行] ダイアログ ボックスを開きます。

1. wsreset.exe と入力し、**[OK]** を選択します。

1. 空のコマンド プロンプト ウィンドウが開きます。 約 10 秒後に、ウィンドウが閉じて、Microsoft Store が自動的に開きます。

**手順 3: Windows Update をリセットする**

1. **[開始]** > **[設定]** > **[更新とセキュリティ]** > **[トラブルシューティング]** の順に選択します。

1. 下にスクロールし、一覧から **[Windows Update]** を選択し、**[トラブルシューティング ツールを実行する]** を選択します。

1. コンピューターを再起動し、問題が引き続き発生するかどうかを確認します。


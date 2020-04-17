---
title: 添付ファイルが大きいために [送信トレイ] に残ってしまう
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241257"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>[送信トレイ] に残っているメッセージを修復する

["メール メッセージの送信、受信、または検索に問題があります"](https://aka.ms/SaRA-OutlookSendReceive) というシナリオを、[Microsoft サポート/回復アシスタント](https://diagnostics.office.com/#/) ツールで実行することから始めるようお勧めします。

メッセージが送信トレイに残ってしまった場合、大きな添付ファイルがあるか、"接続したら直ちに送信する" オプションが有効になっていないことが原因として考えられます。

**大きい添付ファイルを削除する**

1. Outlook で、[**送受信**] >  [**オフライン作業**] の順に選択します。 
2. ナビゲーション ウィンドウで [**送信トレイ**] を選択します。 ここから、以下の操作を行うことができます。 
    - メッセージを削除します (選択してから [**削除**] を選択します)。
    - 下書きフォルダーにメッセージをドラッグし、ダブルクリックして開き、添付ファイルを削除します (選択してから [**削除**] を選択します)。
3. Outlook がメッセージを送信しようとしていることを示すエラーが表示された場合には、Outlook を閉じます。 終了するまでに少し時間がかかる場合があります。 Outlook が終了しない場合は、Ctrl キーと Alt キーを押しながら Del キーを押し、**[タスク マネージャーの起動]** を選択してください。 [タスク マネージャー] の [**プロセス**] タブを選択し、下にスクロールして outlook.exe を選び、[**プロセスの終了**] を選択します。
4. Outlook が終了したら、もう一度起動して手順 2 および 3 を実行します。 
5. 添付ファイルを削除した後で [**送受信**] >  [**オフライン作業**] の順にクリックし、オンライン作業に戻ります。 

[**送信**] をクリックしてもメッセージが [送信トレイ] に残ってしまいますが、ネットワークに接続されていません。 [**送受信**] をクリックして [**オフライン作業**] の状態を確認してください。 青色の場合、ネットワークから切断されています。 クリックして接続してから (ボタンが白に変わります)、[**すべて送信**] をクリックします。
 
**接続したらすぐに送信を有効にする**
 
1. [ファイル] タブの [**オプション**] をクリックします。

2. [Outlook のオプション] ダイアログ ボックスで、[**詳細設定**] をクリックします。

3. [送受信] セクションで [**接続したらすぐに送信**] をクリックして有効にします。 [**OK**] をクリックします。
 
すべての詳細については、以下を参照してください。
- [動画: 残っているメールの送信または削除](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Outlook で送信/受信操作を手動で開始するまで、メールは [送信トレイ] フォルダーに残ります](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)

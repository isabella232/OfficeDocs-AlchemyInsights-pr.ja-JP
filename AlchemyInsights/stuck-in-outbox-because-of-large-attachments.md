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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/10/2019
ms.locfileid: "37443601"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>[送信トレイ] に残っているメッセージを修復する

["メール メッセージの送信、受信、または検索に問題があります"](https://aka.ms/SaRA-OutlookSendReceive) というシナリオを [Microsoft サポート/回復アシスタント](https://diagnostics.office.com/#/) ツールから実行することから開始することをお勧めします。

メッセージが [送信トレイ] に残った場合、最も可能性の高い原因は以下のとおりです。
- 大きい添付ファイル。
- **接続したらすぐに送信**オプションが有効になっていません。

大きい添付ファイルを削除するには: 

1. Outlook で、[**送受信**] >  [**オフライン作業**] の順に選択します。 
2. ナビゲーション ウィンドウで [**送信トレイ**] を選択します。 ここから、以下の操作を行うことができます。 
    - メッセージを削除します (選択してから [**削除**] を選択します)。
    - 下書きフォルダーにメッセージをドラッグし、ダブルクリックして開き、添付ファイルを削除します (選択してから [**削除**] を選択します)。
3. Outlook がメッセージを送信しようとしていることを示すエラーが表示された場合には、Outlook を閉じます。 終了するまでに少し時間がかかる場合があります。 Outlook が終了しない場合は、Ctrl キーと Alt キーを押しながら Del キーを押し、[**タスク マネージャーの起動**] を選択してください。 [タスク マネージャー] の [**プロセス**] タブを選択し、下にスクロールして outlook.exe を選び、[**プロセスの終了**] を選択します。
4. Outlook が終了したら、もう一度起動して手順 2 および 3 を実行します。 
5. 添付ファイルを削除した後で [**送受信**] >  [**オフライン作業**] の順にクリックし、オンライン作業に戻ります。 

[**送信**] をクリックしてもメッセージが [送信トレイ] に残ってしまいますが、ネットワークに接続されていません。 [**送受信**] をクリックして [**オフライン作業**] の状態を確認してください。 青色の場合、ネットワークから切断されています。 選択して接続してから (ボタンが白に変わります)、[**すべて送信**] をクリックします。
 
**接続したらすぐに送信**オプションを有効にするには:
 
- [**ファイル**] >  [**オプション**] >   [**詳細設定**] の順に選択します。
[**送受信**] セクションで [**接続したらすぐに送信**] を選択し、[**OK**] を選択します。
 
すべての詳細については、以下を参照してください。
- [動画: 残っているメールの送信または削除](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Outlook で送信/受信操作を手動で開始するまで、メールは [送信トレイ] フォルダーに残ります](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)

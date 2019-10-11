---
title: 大きな添付ファイルがあるために、送信トレイから動かない
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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/10/2019
ms.locfileid: "37443601"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>送信トレイに残っているメッセージを修正する

[Microsoft サポート/回復アシスタント](https://diagnostics.office.com/#/)ツールを使用して、 ["メールメッセージの送信、受信、または検索で問題](https://aka.ms/SaRA-OutlookSendReceive)が発生しました" というシナリオを実行することをお勧めします。

メッセージが送信トレイに滞留した場合、次の原因が考えられます。
- 大きな添付ファイル。
- [**接続時に直ちに送信する**] オプションが有効になっていない。

大きな添付ファイルを削除するには 

1. Outlook で、[**送受信** > を**オフラインで行う**] を選択します。 
2. ナビゲーションウィンドウで、[**送信トレイ**] を選択します。 ここから、次のことを行うことができます。 
    - メッセージを削除します (選択してから、[**削除**] を選択します)。
    - [下書き] フォルダーにメッセージをドラッグし、ダブルクリックして開き、添付ファイルを削除して、[**削除**] を選択します。
3. Outlook がメッセージを送信しようとしているというエラーが表示された場合は、Outlook を閉じます。 終了するまでしばらく時間がかかる場合があります。 Outlook が終了しない場合は、Ctrl + Alt + Del キーを押して、[**タスクマネージャーの起動**] を選択します。 タスクマネージャーで、[**プロセス**] タブを選択し、[outlook.exe] まで下にスクロールして、[**プロセスの終了**] を選択します。
4. Outlook を閉じた後、再起動して、手順2と3を繰り返します。 
5. 添付ファイルを削除した後、[**オフライン作業**]**をクリックし** > てオンラインで作業を再開します。 

[**送信**] をクリックしたときに、メッセージも送信トレイに残っていますが、接続されていません。 [**送信/受信**] をクリックし、[**オフライン作業**] ボタンを確認します。 青の場合は、切断されています。 接続するものを選択し (ボタンが白に変わります)、[**すべて送信**] をクリックします。
 
**接続時に直ちに送信**を有効にするには:
 
- [**ファイル** > **オプション** >  (**詳細**)] を選択します。
[**送信/受信**] セクションで、[**接続時に直ちに送信する**] を選択し、[ **OK]** を選択します。
 
詳細については、以下を参照してください。
- [ビデオ: スタックメールを送信または削除する](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Outlook で送受信操作を手動で開始しない限り、電子メールは [送信トレイ] フォルダーに残ります。](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)

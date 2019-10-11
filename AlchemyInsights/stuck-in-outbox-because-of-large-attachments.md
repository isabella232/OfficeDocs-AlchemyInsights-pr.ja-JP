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
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="ba825-102">送信トレイに残っているメッセージを修正する</span><span class="sxs-lookup"><span data-stu-id="ba825-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="ba825-103">[Microsoft サポート/回復アシスタント](https://diagnostics.office.com/#/)ツールを使用して、 ["メールメッセージの送信、受信、または検索で問題](https://aka.ms/SaRA-OutlookSendReceive)が発生しました" というシナリオを実行することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="ba825-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="ba825-104">メッセージが送信トレイに滞留した場合、次の原因が考えられます。</span><span class="sxs-lookup"><span data-stu-id="ba825-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="ba825-105">大きな添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="ba825-105">Large attachments.</span></span>
- <span data-ttu-id="ba825-106">[**接続時に直ちに送信する**] オプションが有効になっていない。</span><span class="sxs-lookup"><span data-stu-id="ba825-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="ba825-107">大きな添付ファイルを削除するには</span><span class="sxs-lookup"><span data-stu-id="ba825-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="ba825-108">Outlook で、[**送受信** > を**オフラインで行う**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba825-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="ba825-109">ナビゲーションウィンドウで、[**送信トレイ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba825-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="ba825-110">ここから、次のことを行うことができます。</span><span class="sxs-lookup"><span data-stu-id="ba825-110">From here, you can:</span></span> 
    - <span data-ttu-id="ba825-111">メッセージを削除します (選択してから、[**削除**] を選択します)。</span><span class="sxs-lookup"><span data-stu-id="ba825-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="ba825-112">[下書き] フォルダーにメッセージをドラッグし、ダブルクリックして開き、添付ファイルを削除して、[**削除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba825-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="ba825-113">Outlook がメッセージを送信しようとしているというエラーが表示された場合は、Outlook を閉じます。</span><span class="sxs-lookup"><span data-stu-id="ba825-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="ba825-114">終了するまでしばらく時間がかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="ba825-114">It may take a few moments to exit.</span></span> <span data-ttu-id="ba825-115">Outlook が終了しない場合は、Ctrl + Alt + Del キーを押して、[**タスクマネージャーの起動**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba825-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="ba825-116">タスクマネージャーで、[**プロセス**] タブを選択し、[outlook.exe] まで下にスクロールして、[**プロセスの終了**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba825-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="ba825-117">Outlook を閉じた後、再起動して、手順2と3を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="ba825-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="ba825-118">添付ファイルを削除した後、[**オフライン作業**]**をクリックし** > てオンラインで作業を再開します。</span><span class="sxs-lookup"><span data-stu-id="ba825-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="ba825-119">[**送信**] をクリックしたときに、メッセージも送信トレイに残っていますが、接続されていません。</span><span class="sxs-lookup"><span data-stu-id="ba825-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="ba825-120">[**送信/受信**] をクリックし、[**オフライン作業**] ボタンを確認します。</span><span class="sxs-lookup"><span data-stu-id="ba825-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="ba825-121">青の場合は、切断されています。</span><span class="sxs-lookup"><span data-stu-id="ba825-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="ba825-122">接続するものを選択し (ボタンが白に変わります)、[**すべて送信**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ba825-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="ba825-123">**接続時に直ちに送信**を有効にするには:</span><span class="sxs-lookup"><span data-stu-id="ba825-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="ba825-124">[**ファイル** > **オプション** >  (**詳細**)] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba825-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="ba825-125">[**送信/受信**] セクションで、[**接続時に直ちに送信する**] を選択し、[ **OK]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba825-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="ba825-126">詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba825-126">For full details see:</span></span>
- [<span data-ttu-id="ba825-127">ビデオ: スタックメールを送信または削除する</span><span class="sxs-lookup"><span data-stu-id="ba825-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- <span data-ttu-id="ba825-128">[Outlook で送受信操作を手動で開始しない限り、電子メールは [送信トレイ] フォルダーに残ります。](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)</span><span class="sxs-lookup"><span data-stu-id="ba825-128">[Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)</span></span>

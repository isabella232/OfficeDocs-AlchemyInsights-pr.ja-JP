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
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="942fd-102">[送信トレイ] に残っているメッセージを修復する</span><span class="sxs-lookup"><span data-stu-id="942fd-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="942fd-103">["メール メッセージの送信、受信、または検索に問題があります"](https://aka.ms/SaRA-OutlookSendReceive) というシナリオを [Microsoft サポート/回復アシスタント](https://diagnostics.office.com/#/) ツールから実行することから開始することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="942fd-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="942fd-104">メッセージが [送信トレイ] に残った場合、最も可能性の高い原因は以下のとおりです。</span><span class="sxs-lookup"><span data-stu-id="942fd-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="942fd-105">大きい添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="942fd-105">Large attachments.</span></span>
- <span data-ttu-id="942fd-106">**接続したらすぐに送信**オプションが有効になっていません。</span><span class="sxs-lookup"><span data-stu-id="942fd-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="942fd-107">大きい添付ファイルを削除するには:</span><span class="sxs-lookup"><span data-stu-id="942fd-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="942fd-108">Outlook で、[**送受信**] >  [**オフライン作業**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="942fd-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="942fd-109">ナビゲーション ウィンドウで [**送信トレイ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="942fd-109">In the navigation pane, select **Booking page**.</span></span> <span data-ttu-id="942fd-110">ここから、以下の操作を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="942fd-110">From here, you can:</span></span> 
    - <span data-ttu-id="942fd-111">メッセージを削除します (選択してから [**削除**] を選択します)。</span><span class="sxs-lookup"><span data-stu-id="942fd-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="942fd-112">下書きフォルダーにメッセージをドラッグし、ダブルクリックして開き、添付ファイルを削除します (選択してから [**削除**] を選択します)。</span><span class="sxs-lookup"><span data-stu-id="942fd-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="942fd-113">Outlook がメッセージを送信しようとしていることを示すエラーが表示された場合には、Outlook を閉じます。</span><span class="sxs-lookup"><span data-stu-id="942fd-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="942fd-114">終了するまでに少し時間がかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="942fd-114">It may take a few moments to exit.</span></span> <span data-ttu-id="942fd-115">Outlook が終了しない場合は、Ctrl キーと Alt キーを押しながら Del キーを押し、[**タスク マネージャーの起動**] を選択してください。</span><span class="sxs-lookup"><span data-stu-id="942fd-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="942fd-116">[タスク マネージャー] の [**プロセス**] タブを選択し、下にスクロールして outlook.exe を選び、[**プロセスの終了**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="942fd-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="942fd-117">Outlook が終了したら、もう一度起動して手順 2 および 3 を実行します。</span><span class="sxs-lookup"><span data-stu-id="942fd-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="942fd-118">添付ファイルを削除した後で [**送受信**] >  [**オフライン作業**] の順にクリックし、オンライン作業に戻ります。</span><span class="sxs-lookup"><span data-stu-id="942fd-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="942fd-119">[**送信**] をクリックしてもメッセージが [送信トレイ] に残ってしまいますが、ネットワークに接続されていません。</span><span class="sxs-lookup"><span data-stu-id="942fd-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="942fd-120">[**送受信**] をクリックして [**オフライン作業**] の状態を確認してください。</span><span class="sxs-lookup"><span data-stu-id="942fd-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="942fd-121">青色の場合、ネットワークから切断されています。</span><span class="sxs-lookup"><span data-stu-id="942fd-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="942fd-122">選択して接続してから (ボタンが白に変わります)、[**すべて送信**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="942fd-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="942fd-123">**接続したらすぐに送信**オプションを有効にするには:</span><span class="sxs-lookup"><span data-stu-id="942fd-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="942fd-124">[**ファイル**] >  [**オプション**] >   [**詳細設定**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="942fd-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="942fd-125">[**送受信**] セクションで [**接続したらすぐに送信**] を選択し、[**OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="942fd-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="942fd-126">すべての詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="942fd-126">For details, see:</span></span>
- [<span data-ttu-id="942fd-127">動画: 残っているメールの送信または削除</span><span class="sxs-lookup"><span data-stu-id="942fd-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- <span data-ttu-id="942fd-128">[Outlook で送信/受信操作を手動で開始するまで、メールは [送信トレイ] フォルダーに残ります](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)</span><span class="sxs-lookup"><span data-stu-id="942fd-128">[Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)</span></span>

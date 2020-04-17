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
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="b2927-102">[送信トレイ] に残っているメッセージを修復する</span><span class="sxs-lookup"><span data-stu-id="b2927-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="b2927-103">["メール メッセージの送信、受信、または検索に問題があります"](https://aka.ms/SaRA-OutlookSendReceive) というシナリオを、[Microsoft サポート/回復アシスタント](https://diagnostics.office.com/#/) ツールで実行することから始めるようお勧めします。</span><span class="sxs-lookup"><span data-stu-id="b2927-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="b2927-104">メッセージが送信トレイに残ってしまった場合、大きな添付ファイルがあるか、"接続したら直ちに送信する" オプションが有効になっていないことが原因として考えられます。</span><span class="sxs-lookup"><span data-stu-id="b2927-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="b2927-105">**大きい添付ファイルを削除する**</span><span class="sxs-lookup"><span data-stu-id="b2927-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="b2927-106">Outlook で、[**送受信**] >  [**オフライン作業**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="b2927-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="b2927-107">ナビゲーション ウィンドウで [**送信トレイ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b2927-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="b2927-108">ここから、以下の操作を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="b2927-108">From here, you can:</span></span> 
    - <span data-ttu-id="b2927-109">メッセージを削除します (選択してから [**削除**] を選択します)。</span><span class="sxs-lookup"><span data-stu-id="b2927-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="b2927-110">下書きフォルダーにメッセージをドラッグし、ダブルクリックして開き、添付ファイルを削除します (選択してから [**削除**] を選択します)。</span><span class="sxs-lookup"><span data-stu-id="b2927-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="b2927-111">Outlook がメッセージを送信しようとしていることを示すエラーが表示された場合には、Outlook を閉じます。</span><span class="sxs-lookup"><span data-stu-id="b2927-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="b2927-112">終了するまでに少し時間がかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="b2927-112">It may take a few moments to exit.</span></span> <span data-ttu-id="b2927-113">Outlook が終了しない場合は、Ctrl キーと Alt キーを押しながら Del キーを押し、**[タスク マネージャーの起動]** を選択してください。</span><span class="sxs-lookup"><span data-stu-id="b2927-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="b2927-114">[タスク マネージャー] の [**プロセス**] タブを選択し、下にスクロールして outlook.exe を選び、[**プロセスの終了**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b2927-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="b2927-115">Outlook が終了したら、もう一度起動して手順 2 および 3 を実行します。</span><span class="sxs-lookup"><span data-stu-id="b2927-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="b2927-116">添付ファイルを削除した後で [**送受信**] >  [**オフライン作業**] の順にクリックし、オンライン作業に戻ります。</span><span class="sxs-lookup"><span data-stu-id="b2927-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="b2927-117">[**送信**] をクリックしてもメッセージが [送信トレイ] に残ってしまいますが、ネットワークに接続されていません。</span><span class="sxs-lookup"><span data-stu-id="b2927-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="b2927-118">[**送受信**] をクリックして [**オフライン作業**] の状態を確認してください。</span><span class="sxs-lookup"><span data-stu-id="b2927-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="b2927-119">青色の場合、ネットワークから切断されています。</span><span class="sxs-lookup"><span data-stu-id="b2927-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="b2927-120">クリックして接続してから (ボタンが白に変わります)、[**すべて送信**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b2927-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="b2927-121">**接続したらすぐに送信を有効にする**</span><span class="sxs-lookup"><span data-stu-id="b2927-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="b2927-122">[ファイル] タブの [**オプション**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b2927-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="b2927-123">[Outlook のオプション] ダイアログ ボックスで、[**詳細設定**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b2927-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="b2927-124">[送受信] セクションで [**接続したらすぐに送信**] をクリックして有効にします。</span><span class="sxs-lookup"><span data-stu-id="b2927-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="b2927-125">[**OK**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b2927-125">Click **OK**.</span></span>
 
<span data-ttu-id="b2927-126">すべての詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2927-126">For full details, see:</span></span>
- [<span data-ttu-id="b2927-127">動画: 残っているメールの送信または削除</span><span class="sxs-lookup"><span data-stu-id="b2927-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- <span data-ttu-id="b2927-128">[Outlook で送信/受信操作を手動で開始するまで、メールは [送信トレイ] フォルダーに残ります](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)</span><span class="sxs-lookup"><span data-stu-id="b2927-128">[Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)</span></span>

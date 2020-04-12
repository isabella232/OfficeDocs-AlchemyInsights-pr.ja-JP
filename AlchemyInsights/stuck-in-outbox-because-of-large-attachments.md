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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232635"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="292be-102">[送信トレイ] に残っているメッセージを修復する</span><span class="sxs-lookup"><span data-stu-id="292be-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="292be-103">["メール メッセージの送信、受信、または検索に問題があります"](https://aka.ms/SaRA-OutlookSendReceive) というシナリオを、影響を受けているコンピューターの [Microsoft サポート/回復アシスタント](https://diagnostics.office.com/#/) ツールから実行することから開始することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="292be-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="292be-104">メッセージが送信トレイに残ってしまった場合、大きな添付ファイルがあるか、"接続したら直ちに送信する" オプションが有効になっていないことが原因として考えられます。</span><span class="sxs-lookup"><span data-stu-id="292be-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="292be-105">**大きい添付ファイルを削除する**</span><span class="sxs-lookup"><span data-stu-id="292be-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="292be-106">[**送受信**] > [**オフライン作業**] の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="292be-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="292be-107">ナビゲーション ウィンドウの [**送信トレイ**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="292be-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="292be-108">ここから、以下の操作を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="292be-108">From here, you can:</span></span> 
    - <span data-ttu-id="292be-109">メッセージを削除する。</span><span class="sxs-lookup"><span data-stu-id="292be-109">Delete the message.</span></span> <span data-ttu-id="292be-110">メッセージを選択し、[**削除**] をクリックするだけです。</span><span class="sxs-lookup"><span data-stu-id="292be-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="292be-111">メッセージを**下書きフォルダー**にドラッグし、ダブルクリックして開いてから、添付ファイルを削除します (添付ファイルをクリックし、[**削除**] をクリックします)。</span><span class="sxs-lookup"><span data-stu-id="292be-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="292be-112">Outlook がメッセージを送信しようとしていることを示すエラーが表示された場合には、Outlook を閉じます。</span><span class="sxs-lookup"><span data-stu-id="292be-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="292be-113">終了するまでに少し時間がかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="292be-113">It may take a few moments to exit.</span></span> <span data-ttu-id="292be-114">Outlook が終了しない場合は、**Ctrl キーと Alt キーを押しながら Del キーを押し**、[**タスク マネージャーの起動**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="292be-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="292be-115">[タスク マネージャー] の [**プロセス**] タブを選択し、下にスクロールして outlook.exe を選び、[**プロセスの終了**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="292be-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="292be-116">Outlook が終了したら、もう一度 Outlook 起動し、手順 2 から 3 を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="292be-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="292be-117">添付ファイルを削除した後で [**送受信**] > [**オフライン作業**] の順にクリックしてボタンの選択を解除し、オンライン作業に戻ります。</span><span class="sxs-lookup"><span data-stu-id="292be-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="292be-118">[**送信**] をクリックしてもメッセージが [送信トレイ] に残ってしまいますが、ネットワークに接続されていません。</span><span class="sxs-lookup"><span data-stu-id="292be-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="292be-119">[**送受信**] をクリックして [**オフライン作業**] の状態を確認してください。</span><span class="sxs-lookup"><span data-stu-id="292be-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="292be-120">青色の場合、ネットワークから切断されています。</span><span class="sxs-lookup"><span data-stu-id="292be-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="292be-121">クリックして接続してから (ボタンが白に変わります)、[**すべて送信**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="292be-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="292be-122">**接続したらすぐに送信を有効にする**</span><span class="sxs-lookup"><span data-stu-id="292be-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="292be-123">[ファイル] タブの [**オプション**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="292be-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="292be-124">[Outlook のオプション] ダイアログ ボックスで、[**詳細設定**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="292be-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="292be-125">[送受信] セクションで [**接続したらすぐに送信**] をクリックして有効にします。</span><span class="sxs-lookup"><span data-stu-id="292be-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="292be-126">[**OK**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="292be-126">Click **OK**.</span></span>
 
<span data-ttu-id="292be-127">すべての詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="292be-127">For full details, see:</span></span>
- [<span data-ttu-id="292be-128">動画: 残っているメールの送信または削除</span><span class="sxs-lookup"><span data-stu-id="292be-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- <span data-ttu-id="292be-129">[Outlook で送信/受信操作を手動で開始するまで、メールは [送信トレイ] フォルダーに残ります](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)</span><span class="sxs-lookup"><span data-stu-id="292be-129">[Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)</span></span>

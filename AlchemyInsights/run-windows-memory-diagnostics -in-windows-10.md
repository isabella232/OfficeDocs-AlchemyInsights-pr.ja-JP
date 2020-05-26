---
title: Windows 10 の Windows メモリ診断を実行する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358719"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="a10b3-102">Windows 10 の Windows メモリ診断を実行する</span><span class="sxs-lookup"><span data-stu-id="a10b3-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="a10b3-103">PC の Windows およびアプリがクラッシュしたり、フリーズしたり動作が不安定になったりする場合、PC のメモリ (RAM) に問題がある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a10b3-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="a10b3-104">Windows メモリ診断を実行して、PC の RAM に問題があるかどうかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="a10b3-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="a10b3-105">タスクバーの検索ボックスに **「メモリ診断」** と入力し、**[Windows メモリ診断]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a10b3-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="a10b3-106">診断を実行するには、PC の再起動が必要です。</span><span class="sxs-lookup"><span data-stu-id="a10b3-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="a10b3-107">すぐに再起動するか、(作業内容を保存して、開いているドキュメントと電子メールを先に終了します)。または、次回 PC が再起動したときに自動的に実行されるように診断をスケジュールすることができます。</span><span class="sxs-lookup"><span data-stu-id="a10b3-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows メモリ診断](media/windows-memory-diagnostic.png)

<span data-ttu-id="a10b3-109">PC が再起動すると、\*\* Windows メモリ診断ツール\*\*が自動的に実行されます。</span><span class="sxs-lookup"><span data-stu-id="a10b3-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="a10b3-110">診断実行時に状態と進捗状況が表示されます。また、使用しているキーボードの **ESC** キーを押して診断をキャンセルすることもできます。</span><span class="sxs-lookup"><span data-stu-id="a10b3-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="a10b3-111">診断が完了すると、Windows は正常に起動します。</span><span class="sxs-lookup"><span data-stu-id="a10b3-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="a10b3-112">再起動した直後にデスクトップが表示されると、(**アクションセンター**のタスク センターのアイコンの横) メモリ エラーが検出されたかどうかを示す通知が表示されます。</span><span class="sxs-lookup"><span data-stu-id="a10b3-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="a10b3-113">例:</span><span class="sxs-lookup"><span data-stu-id="a10b3-113">For example:</span></span>

<span data-ttu-id="a10b3-114">アクション センターのアイコン:</span><span class="sxs-lookup"><span data-stu-id="a10b3-114">Here's the Action Center icon:</span></span> ![アクション センターアイコン](media/action-center-icon.png) 

<span data-ttu-id="a10b3-116">通知のサンプル:</span><span class="sxs-lookup"><span data-stu-id="a10b3-116">And a sample notification:</span></span> ![メモリ エラーはありません](media/no-memory-errors.png)

<span data-ttu-id="a10b3-118">通知を見逃した場合は、タスクバーの **[アクション センター]** アイコンを選択 し、**アクション センター**を表示して スクロール可能な通知の一覧を表示することができます。</span><span class="sxs-lookup"><span data-stu-id="a10b3-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="a10b3-119">詳細情報を確認するには、タスクバーの検索ボックスに **「イベント」** と入力して、**[イベントビューアー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a10b3-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="a10b3-120">**イベントビューアー**の左側のウィンドウで、**[Windows ログ]、[ システム]** に移動 ます。</span><span class="sxs-lookup"><span data-stu-id="a10b3-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="a10b3-121">右側のウィンドウで、Source 値 **"MemoryDiagnostics-結果"** のイベントが表示されるまで **[ソース]** 列を見ながら一覧を下にスキャンします。</span><span class="sxs-lookup"><span data-stu-id="a10b3-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="a10b3-122">それぞれのイベントを強調表示し、一覧の下にある **[全般]** タブ の下のボックスに結果情報を表示します。</span><span class="sxs-lookup"><span data-stu-id="a10b3-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>

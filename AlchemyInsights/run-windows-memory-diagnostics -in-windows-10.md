---
title: Windows 10 の Windows メモリ診断を実行する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826672"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="96805-102">Windows 10 の Windows メモリ診断を実行する</span><span class="sxs-lookup"><span data-stu-id="96805-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="96805-103">PC の Windows およびアプリがクラッシュしたり、フリーズしたり動作が不安定になったりする場合、PC のメモリ (RAM) に問題がある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="96805-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="96805-104">Windows メモリ診断を実行して、PC の RAM に問題があるかどうかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="96805-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="96805-105">タスクバーの検索ボックスに **「メモリ診断」** と入力し、**[Windows メモリ診断]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="96805-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="96805-106">診断を実行するには、PC の再起動が必要です。</span><span class="sxs-lookup"><span data-stu-id="96805-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="96805-107">すぐに再起動するか、(作業内容を保存して、開いているドキュメントと電子メールを先に終了します)。または、次回 PC が再起動したときに自動的に実行されるように診断をスケジュールすることができます。</span><span class="sxs-lookup"><span data-stu-id="96805-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows メモリ診断](media/windows-memory-diagnostic.png)

<span data-ttu-id="96805-109">PC が再起動すると、**Windows メモリ診断ツール** が自動的に実行されます。</span><span class="sxs-lookup"><span data-stu-id="96805-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="96805-110">診断実行時に状態と進捗状況が表示されます。また、使用しているキーボードの **ESC** キーを押して診断をキャンセルすることもできます。</span><span class="sxs-lookup"><span data-stu-id="96805-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="96805-111">診断が完了すると、Windows は正常に起動します。</span><span class="sxs-lookup"><span data-stu-id="96805-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="96805-112">再起動した直後にデスクトップが表示されると、(**アクションセンター** のタスク センターのアイコンの横) メモリ エラーが検出されたかどうかを示す通知が表示されます。</span><span class="sxs-lookup"><span data-stu-id="96805-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="96805-113">例:</span><span class="sxs-lookup"><span data-stu-id="96805-113">For example:</span></span>

<span data-ttu-id="96805-114">アクション センターのアイコン:</span><span class="sxs-lookup"><span data-stu-id="96805-114">Here's the Action Center icon:</span></span> ![アクション センターアイコン](media/action-center-icon.png) 

<span data-ttu-id="96805-116">通知のサンプル:</span><span class="sxs-lookup"><span data-stu-id="96805-116">And a sample notification:</span></span> ![メモリ エラーはありません](media/no-memory-errors.png)

<span data-ttu-id="96805-118">通知を見逃した場合は、タスクバーの **[アクション センター]** アイコンを選択 し、**アクション センター** を表示して スクロール可能な通知の一覧を表示することができます。</span><span class="sxs-lookup"><span data-stu-id="96805-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="96805-119">詳細情報を確認するには、タスクバーの検索ボックスに **「イベント」** と入力して、**[イベントビューアー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="96805-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="96805-120">**イベントビューアー** の左側のウィンドウで、**[Windows ログ]、[ システム]** に移動 ます。</span><span class="sxs-lookup"><span data-stu-id="96805-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="96805-121">右側のウィンドウで、Source 値 **"MemoryDiagnostics-結果"** のイベントが表示されるまで **[ソース]** 列を見ながら一覧を下にスキャンします。</span><span class="sxs-lookup"><span data-stu-id="96805-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="96805-122">それぞれのイベントを強調表示し、一覧の下にある **[全般]** タブ の下のボックスに結果情報を表示します。</span><span class="sxs-lookup"><span data-stu-id="96805-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>

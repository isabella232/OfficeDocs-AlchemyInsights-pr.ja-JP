---
title: 予定表イベントが表示されない、または更新されない
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837686"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="157b1-102">予定表イベントが表示されない、または更新されない</span><span class="sxs-lookup"><span data-stu-id="157b1-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="157b1-103">予定表アイテムが表示されない、または更新されない場合は、Outlook の [予定表] フォルダーのプロパティにあるアイテム数の確認から始めます。</span><span class="sxs-lookup"><span data-stu-id="157b1-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="157b1-104">影響を受けたユーザーの **[予定表]** フォルダーを右クリックし、**[プロパティ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="157b1-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="157b1-105">**[同期]** タブを選択します。</span><span class="sxs-lookup"><span data-stu-id="157b1-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="157b1-106">[サーバー] フォルダーと [オフライン] フォルダーの間でアイテム数が同じではない場合は次のように操作します。</span><span class="sxs-lookup"><span data-stu-id="157b1-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="157b1-107">**[予定表]** フォルダーを強調表示します。</span><span class="sxs-lookup"><span data-stu-id="157b1-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="157b1-108">**[送信]**/**[受信]** タブに移動し、**[フォルダーを更新する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="157b1-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="157b1-109">予定表がまだ更新されないか、イベントが表示されない場合は、[Microsoft ダウンロード センター](https://www.microsoft.com/download/details.aspx?id=28786)から Outlook 用予定表チェック ツールをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="157b1-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="157b1-110">予定表フォルダーに 5000 個を超えるアイテムが含まれるかどうかを確認します。これが原因で、予定表会議が更新されない現象や会議のエラーなどが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="157b1-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="157b1-111">詳細については、「[キャッシュ モードの .ost ファイルまたは .pst ファイル内のアイテムまたはフォルダーが多すぎる場合の Outlook のパフォーマンスの問題](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="157b1-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>
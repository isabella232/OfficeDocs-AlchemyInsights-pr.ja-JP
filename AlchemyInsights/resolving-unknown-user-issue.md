---
title: Teams チャットの不明なユーザーの問題の解決
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003807"
- "6809"
ms.openlocfilehash: 523c11cb9d5c4696703c67c2a6b3184f5d12f8e7
ms.sourcegitcommit: d151b09064df3fb573ae07a387a08d98a9553b9b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808201"
---
# <a name="resolving-issue-with-unknown-user-in-teams-chat"></a><span data-ttu-id="00a4e-102">Teams チャットの「不明なユーザー」の問題の解決</span><span class="sxs-lookup"><span data-stu-id="00a4e-102">Resolving issue with "Unknown User" in Teams Chat</span></span>

<span data-ttu-id="00a4e-103">削除されたユーザーが「不明なユーザー」として表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="00a4e-103">At times, a removed user will appear as "Unknown User".</span></span> <span data-ttu-id="00a4e-104">これは[既知の問題](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown)です。</span><span class="sxs-lookup"><span data-stu-id="00a4e-104">This is a [known issue](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span></span>

<span data-ttu-id="00a4e-105">Teams チャットでユーザーが「不明なユーザー」として表示され続ける場合は、キャッシュをクリアしてみてください。</span><span class="sxs-lookup"><span data-stu-id="00a4e-105">If you are persistently seeing users showing as "Unknown User" in Teams chats, try and clear the cache:</span></span>

1.  <span data-ttu-id="00a4e-106">タスクバーの [Teams] アイコンを右クリックします。</span><span class="sxs-lookup"><span data-stu-id="00a4e-106">Right-click the Teams icon in the taskbar.</span></span> <span data-ttu-id="00a4e-107">**[終了]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="00a4e-107">Click  **Quit**.</span></span>
2.  <span data-ttu-id="00a4e-108">コンピューターの %appdata%\Microsoft\teams\ フォルダーに移動して、そのディレクトリにあるすべてのファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="00a4e-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>

<span data-ttu-id="00a4e-109">匿名ユーザーがロビーで待機するようにすることで、匿名ユーザーが会議に参加するのを防ぐことができます。</span><span class="sxs-lookup"><span data-stu-id="00a4e-109">You can prevent anonymous users from joining meetings by ensuring that they wait in the lobby.</span></span> <span data-ttu-id="00a4e-110">詳しくは、「[Teams 会議の参加者設定を変更する](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00a4e-110">For more information, see [Change participant settings for a Teams meeting](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).</span></span>

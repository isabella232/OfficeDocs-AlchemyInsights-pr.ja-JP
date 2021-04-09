---
title: Teams チャットで共有されているファイルにアクセスできない
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 5290b1eea907fc5b785c20654d92467a4ed0af04
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/02/2021
ms.locfileid: "51596092"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a><span data-ttu-id="ad1f6-102">Teams チャットで共有されているファイルにアクセスできない</span><span class="sxs-lookup"><span data-stu-id="ad1f6-102">Unable to access files shared in Teams chat</span></span>

<span data-ttu-id="ad1f6-103">Microsoft Teams では、チャット ウィンドウでユーザーが共有したファイルは、共有ユーザーの OneDrive サイトに自動的に保存されます。</span><span class="sxs-lookup"><span data-stu-id="ad1f6-103">In Microsoft Teams, a file shared by a user in a chat window is stored automatically on the sharing user's OneDrive site.</span></span>

<span data-ttu-id="ad1f6-104">他のユーザーが Teams でファイルを開こうとしたときに "このファイルへのアクセス権がありません" というエラー メッセージが表示される場合、この問題は、制限付きアクセス ユーザーのアクセス許可ロックダウン モード機能が OneDrive サイトで有効になっていることが原因で発生しています。</span><span class="sxs-lookup"><span data-stu-id="ad1f6-104">When another user tries to open the file in Teams and receives the error message "You don't have access to this file," the issue occurs because the Limited-access user permission lockdown mode feature is activated on your OneDrive site.</span></span>

1. <span data-ttu-id="ad1f6-105">OneDrive サイトで機能を無効にする方法については、「[Error when opening a file in Teams (Teams でファイルを開くときのエラー)](https://go.microsoft.com/fwlink/?linkid=2155733)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad1f6-105">For instructions to disable the feature on the OneDrive site, see [Error when opening a file in Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span></span>

1. <span data-ttu-id="ad1f6-106">他のユーザーが OneDrive サイトへのアクセス権を持っているかどうかを確認し、「[OneDrive のファイルとフォルダーの共有](https://go.microsoft.com/fwlink/?linkid=2156017)」の手順に従ってアクセス権を付与します。</span><span class="sxs-lookup"><span data-stu-id="ad1f6-106">Check whether another user has access to the OneDrive site, and provide access by following the instructions in [Share OneDrive files and folders](https://go.microsoft.com/fwlink/?linkid=2156017).</span></span>
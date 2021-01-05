---
title: ハードコーディングされたパスではなく、データ ディレクトリ変数を使用して Microsoft Edge を変更する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/09/2020
ms.locfileid: "49680479"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a><span data-ttu-id="0eabd-102">ハードコーディングされたパスではなく、データ ディレクトリ変数を使用して Microsoft Edge を変更する</span><span class="sxs-lookup"><span data-stu-id="0eabd-102">Modify Microsoft Edge by using data directory variables rather than hardcoded paths</span></span>

<span data-ttu-id="0eabd-103">たとえば、Windows では、プロファイル データを既定の場所ではなく、ユーザーのローカル アプリケーション データに格納するには、**UserDataDir** ポリシーを **${local_app_data}\Edge\Profile** に設定します。</span><span class="sxs-lookup"><span data-stu-id="0eabd-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the **UserDataDir** policy to **${local_app_data}\Edge\Profile**.</span></span> 

<span data-ttu-id="0eabd-104">詳細については、「[Microsoft Edge ユーザー データ ディレクトリ変数を作成する](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0eabd-104">To learn more, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span></span>
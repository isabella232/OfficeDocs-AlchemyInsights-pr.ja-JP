---
title: Teams クライアントがクラッシュした場合
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2020
ms.locfileid: "43040224"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="981b3-102">Teams クライアントがクラッシュした場合</span><span class="sxs-lookup"><span data-stu-id="981b3-102">Teams client crashing?</span></span>

<span data-ttu-id="981b3-103">Teams クライアントがクラッシュした場合は、次のことを実施してください。</span><span class="sxs-lookup"><span data-stu-id="981b3-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="981b3-104">Teams デスクトップ アプリを使用している場合は、[アプリが完全に更新されていることを確認します](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。</span><span class="sxs-lookup"><span data-stu-id="981b3-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="981b3-105">すべての [Office 365 の URL とアドレスの範囲](https://docs.microsoft.com/microsoftteams/connectivity-issues)にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="981b3-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="981b3-106">管理者アカウントでログインし、[サービス正常性ダッシュボード](https://docs.microsoft.com/office365/enterprise/view-service-health)をチェックして、停止やサービスの低下がないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="981b3-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="981b3-107">最後の手順として、以下の操作を実行して Teams クライアントのキャッシュをクリアします。</span><span class="sxs-lookup"><span data-stu-id="981b3-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="981b3-108">Microsoft Teams デスクトップ クライアントを完全に終了します。</span><span class="sxs-lookup"><span data-stu-id="981b3-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="981b3-109">トレイのアイコンから **Teams** を右クリックして **[終了]** をクリックするか、タスク マネージャーを実行してプロセスを完全に強制終了します。</span><span class="sxs-lookup"><span data-stu-id="981b3-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="981b3-110">エクスプローラーに移動し、%appdata%\Microsoft\teams と入力します。</span><span class="sxs-lookup"><span data-stu-id="981b3-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="981b3-111">ディレクトリには、次のようなフォルダーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="981b3-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="981b3-112">**Application Cache** から、Cache に移動し、Cache の場所 (%appdata%\Microsoft\teams\application cache\cache) にあるすべてのファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="981b3-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="981b3-113">**Blob_storage** (%appdata%\Microsoft\teams\blob_storage) から、すべてのファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="981b3-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="981b3-114">**Cache** (%appdata%\Microsoft\teams\Cache) から、すべてのファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="981b3-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="981b3-115">**databases** (%appdata%\Microsoft\teams\databases) から、すべてのファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="981b3-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="981b3-116">**GPUCache** (%appdata%\Microsoft\teams\GPUcache) から、すべてのファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="981b3-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="981b3-117">**IndexedDB** (%appdata%\Microsoft\teams\IndexedDB) から、db ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="981b3-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="981b3-118">**Local Storage** (%appdata%\Microsoft\teams\Local Storage) から、すべてのファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="981b3-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="981b3-119">最後に、**tmp** (%appdata%\Microsoft\teams\tmp) から、すべてのファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="981b3-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="981b3-120">Teams クライアントを再起動します。</span><span class="sxs-lookup"><span data-stu-id="981b3-120">Restart your Teams client.</span></span>

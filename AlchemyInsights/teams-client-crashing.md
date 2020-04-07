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
# <a name="teams-client-crashing"></a>Teams クライアントがクラッシュした場合

Teams クライアントがクラッシュした場合は、次のことを実施してください。

- Teams デスクトップ アプリを使用している場合は、[アプリが完全に更新されていることを確認します](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。

- すべての [Office 365 の URL とアドレスの範囲](https://docs.microsoft.com/microsoftteams/connectivity-issues)にアクセスできることを確認します。

- 管理者アカウントでログインし、[サービス正常性ダッシュボード](https://docs.microsoft.com/office365/enterprise/view-service-health)をチェックして、停止やサービスの低下がないことを確認します。

 - 最後の手順として、以下の操作を実行して Teams クライアントのキャッシュをクリアします。

    1.  Microsoft Teams デスクトップ クライアントを完全に終了します。 トレイのアイコンから **Teams** を右クリックして **[終了]** をクリックするか、タスク マネージャーを実行してプロセスを完全に強制終了します。

    2.  エクスプローラーに移動し、%appdata%\Microsoft\teams と入力します。

    3.  ディレクトリには、次のようなフォルダーが表示されます。

         - **Application Cache** から、Cache に移動し、Cache の場所 (%appdata%\Microsoft\teams\application cache\cache) にあるすべてのファイルを削除します。

        - **Blob_storage** (%appdata%\Microsoft\teams\blob_storage) から、すべてのファイルを削除します。

        - **Cache** (%appdata%\Microsoft\teams\Cache) から、すべてのファイルを削除します。

        - **databases** (%appdata%\Microsoft\teams\databases) から、すべてのファイルを削除します。

        - **GPUCache** (%appdata%\Microsoft\teams\GPUcache) から、すべてのファイルを削除します。

        - **IndexedDB** (%appdata%\Microsoft\teams\IndexedDB) から、db ファイルを削除します。

        - **Local Storage** (%appdata%\Microsoft\teams\Local Storage) から、すべてのファイルを削除します。

        - 最後に、**tmp** (%appdata%\Microsoft\teams\tmp) から、すべてのファイルを削除します。

    4. Teams クライアントを再起動します。

---
title: Teams クライアントがクラッシュした場合
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691112"
---
# <a name="teams-client-crashing"></a>Teams クライアントがクラッシュした場合

Teams クライアントがクラッシュした場合は、次のことを実施してください。

- Teams デスクトップ アプリを使用している場合は、[アプリが完全に更新されていることを確認します](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。

- すべての [Microsoft 365 の URL とアドレスの範囲](https://docs.microsoft.com/microsoftteams/connectivity-issues)にアクセスできることを確認します。

- テナント管理者アカウントでログインし、[サービス正常性ダッシュボード](https://docs.microsoft.com/office365/enterprise/view-service-health)をチェックして、停止やサービスの低下がないことを確認します。

- Teams アプリケーションをアンインストールして再インストールする (リンク)
    - コンピューターの %appdata%\Microsoft\teams\ フォルダーに移動して、そのディレクトリにあるすべてのファイルを削除します。
    - [Teams アプリをダウンロードしてインストールします](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)。可能であれば、管理者として Teams をインストールします (Teams インストーラーを右クリックし、利用可能な場合は [管理者として実行] を選択します)。

Teams クライアントがまだクラッシュする場合、問題を再現することができますか? その場合には、以下の手順を行います。

1. ステップ記録ツールを使用して、手順をキャプチャします。
    - 不要なアプリケーションや機密のアプリケーションをすべて閉じます。
    - ステップ記録ツールを起動し、影響を受けているユーザー アカウントを使用してログインした状態で、問題を再現します。
    - [記録された再現手順をキャプチャする Teams ログを収集します](https://docs.microsoft.com/microsoftteams/log-files)。 **注**: 影響を受けているユーザーのサインイン アドレスがキャプチャされていることを確認します。
    - ダンプや障害バケット情報 (Windows) を収集します。 クラッシュが発生しているコンピューターで Windows Powershell を起動し、次のコマンドを実行します。

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. サポート ケースにファイルを添付します。

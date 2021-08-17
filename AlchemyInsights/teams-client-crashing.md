---
title: Teams クライアントのクラッシュ
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
- "9002323"
- "4512"
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890343"
---
# <a name="teams-client-crashing"></a>Teams クライアントのクラッシュ

Teams クライアントがクラッシュした場合は、次のことを実施してください。

- Teams デスクトップ アプリを使用している場合は、[アプリが完全に更新されていることを確認します](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。

- すべての [Microsoft 365 の URL とアドレスの範囲](https://docs.microsoft.com/microsoftteams/connectivity-issues)にアクセスできることを確認します。

- テナント管理者アカウントでログインし、[サービス正常性ダッシュボード](https://docs.microsoft.com/office365/enterprise/view-service-health)をチェックして、停止やサービスの低下がないことを確認します。

- Teams アプリケーションをアンインストールして再インストールする
    - コンピューターの %appdata%\Microsoft\teams\ フォルダーに移動して、そのディレクトリにあるすべてのファイルを削除します。
    - [Teams アプリをダウンロードしてインストール](https://www.microsoft.com/microsoft-teams/download-app)し、可能であれば、管理者として Teams をインストールします (Teams インストーラーを右クリックし、利用可能な場合は [**管理者として実行**] を選択します)。

Teams クライアントがそれでもまだクラッシュする場合、その問題を再現を試みてください。可能な場合:

1. ステップ記録ツールを使用して、手順をキャプチャします。
    - 不要なアプリケーションや機密のアプリケーションをすべて閉じます。
    - ステップ記録ツールを起動し、影響を受けているユーザー アカウントを使用してログインした状態で、問題を再現します。
    - [記録された再現手順をキャプチャする Teams ログを収集します](https://docs.microsoft.com/microsoftteams/log-files)。 **注**: 影響を受けているユーザーのサインイン アドレスがキャプチャされていることを確認します。
    - ダンプや障害バケット情報 (Windows) を収集します。クラッシュが発生しているコンピューターで Windows Powershell を起動し、次のコマンドを実行します (各コマンドの後に Enter キーを押します):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. テキスト ファイルが生成され、画面に表示されたら、ファイルを保存してサービス要求に添付します。 

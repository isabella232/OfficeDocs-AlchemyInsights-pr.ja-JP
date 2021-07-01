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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187726"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="b6d70-102">Teams クライアントのクラッシュ</span><span class="sxs-lookup"><span data-stu-id="b6d70-102">Teams client crashing</span></span>

<span data-ttu-id="b6d70-103">Teams クライアントがクラッシュした場合は、次のことを実施してください。</span><span class="sxs-lookup"><span data-stu-id="b6d70-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="b6d70-104">Teams デスクトップ アプリを使用している場合は、[アプリが完全に更新されていることを確認します](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。</span><span class="sxs-lookup"><span data-stu-id="b6d70-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="b6d70-105">すべての [Microsoft 365 の URL とアドレスの範囲](/microsoftteams/connectivity-issues)にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b6d70-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="b6d70-106">テナント管理者アカウントでログインし、[サービス正常性ダッシュボード](/office365/enterprise/view-service-health)をチェックして、停止やサービスの低下がないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="b6d70-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="b6d70-107">Teams アプリケーションをアンインストールして再インストールする</span><span class="sxs-lookup"><span data-stu-id="b6d70-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="b6d70-108">コンピューターの %appdata%\Microsoft\teams\ フォルダーに移動して、そのディレクトリにあるすべてのファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="b6d70-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="b6d70-109">[Teams アプリをダウンロードしてインストール](https://www.microsoft.com/microsoft-teams/download-app)し、可能であれば、管理者として Teams をインストールします (Teams インストーラーを右クリックし、利用可能な場合は [**管理者として実行**] を選択します)。</span><span class="sxs-lookup"><span data-stu-id="b6d70-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="b6d70-110">Teams クライアントがそれでもまだクラッシュする場合、その問題を再現を試みてください。</span><span class="sxs-lookup"><span data-stu-id="b6d70-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="b6d70-111">可能な場合:</span><span class="sxs-lookup"><span data-stu-id="b6d70-111">If you can:</span></span>

1. <span data-ttu-id="b6d70-112">ステップ記録ツールを使用して、手順をキャプチャします。</span><span class="sxs-lookup"><span data-stu-id="b6d70-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="b6d70-113">不要なアプリケーションや機密のアプリケーションをすべて閉じます。</span><span class="sxs-lookup"><span data-stu-id="b6d70-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="b6d70-114">ステップ記録ツールを起動し、影響を受けているユーザー アカウントを使用してログインした状態で、問題を再現します。</span><span class="sxs-lookup"><span data-stu-id="b6d70-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="b6d70-115">[記録された再現手順をキャプチャする Teams ログを収集します](/microsoftteams/log-files)。</span><span class="sxs-lookup"><span data-stu-id="b6d70-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="b6d70-116">**注**: 影響を受けているユーザーのサインイン アドレスがキャプチャされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b6d70-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="b6d70-117">ダンプや障害バケット情報 (Windows) を収集します。</span><span class="sxs-lookup"><span data-stu-id="b6d70-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="b6d70-118">クラッシュが発生しているコンピューターで Windows Powershell を起動し、次のコマンドを実行します (各コマンドの後に Enter キーを押します):</span><span class="sxs-lookup"><span data-stu-id="b6d70-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="b6d70-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="b6d70-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="b6d70-120">テキスト ファイルが生成され、画面に表示されたら、ファイルを保存してサービス要求に添付します。</span><span class="sxs-lookup"><span data-stu-id="b6d70-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 

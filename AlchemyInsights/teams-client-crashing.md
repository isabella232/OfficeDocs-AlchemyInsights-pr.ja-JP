---
title: Teams クライアントがクラッシュした場合
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
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826276"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="4d342-102">Teams クライアントがクラッシュした場合</span><span class="sxs-lookup"><span data-stu-id="4d342-102">Teams client crashing?</span></span>

<span data-ttu-id="4d342-103">Teams クライアントがクラッシュした場合は、次のことを実施してください。</span><span class="sxs-lookup"><span data-stu-id="4d342-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="4d342-104">Teams デスクトップ アプリを使用している場合は、[アプリが完全に更新されていることを確認します](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。</span><span class="sxs-lookup"><span data-stu-id="4d342-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="4d342-105">すべての [Microsoft 365 の URL とアドレスの範囲](https://docs.microsoft.com/microsoftteams/connectivity-issues)にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="4d342-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="4d342-106">テナント管理者アカウントでログインし、[サービス正常性ダッシュボード](https://docs.microsoft.com/office365/enterprise/view-service-health)をチェックして、停止やサービスの低下がないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="4d342-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="4d342-107">Teams アプリケーションをアンインストールして再インストールする (リンク)</span><span class="sxs-lookup"><span data-stu-id="4d342-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="4d342-108">コンピューターの %appdata%\Microsoft\teams\ フォルダーに移動して、そのディレクトリにあるすべてのファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="4d342-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="4d342-109">[Teams アプリをダウンロードしてインストールします](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)。可能であれば、管理者として Teams をインストールします (Teams インストーラーを右クリックし、利用可能な場合は [管理者として実行] を選択します)。</span><span class="sxs-lookup"><span data-stu-id="4d342-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="4d342-110">Teams クライアントがまだクラッシュする場合、問題を再現することができますか?</span><span class="sxs-lookup"><span data-stu-id="4d342-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="4d342-111">その場合には、以下の手順を行います。</span><span class="sxs-lookup"><span data-stu-id="4d342-111">If so:</span></span>

1. <span data-ttu-id="4d342-112">ステップ記録ツールを使用して、手順をキャプチャします。</span><span class="sxs-lookup"><span data-stu-id="4d342-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="4d342-113">不要なアプリケーションや機密のアプリケーションをすべて閉じます。</span><span class="sxs-lookup"><span data-stu-id="4d342-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="4d342-114">ステップ記録ツールを起動し、影響を受けているユーザー アカウントを使用してログインした状態で、問題を再現します。</span><span class="sxs-lookup"><span data-stu-id="4d342-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="4d342-115">[記録された再現手順をキャプチャする Teams ログを収集します](https://docs.microsoft.com/microsoftteams/log-files)。</span><span class="sxs-lookup"><span data-stu-id="4d342-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="4d342-116">**注**: 影響を受けているユーザーのサインイン アドレスがキャプチャされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="4d342-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="4d342-117">ダンプや障害バケット情報 (Windows) を収集します。</span><span class="sxs-lookup"><span data-stu-id="4d342-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="4d342-118">クラッシュが発生しているコンピューターで Windows Powershell を起動し、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="4d342-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="4d342-119">サポート ケースにファイルを添付します。</span><span class="sxs-lookup"><span data-stu-id="4d342-119">Attach the file to your support case.</span></span>

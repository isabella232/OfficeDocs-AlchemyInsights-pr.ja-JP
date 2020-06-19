---
title: Microsoft 365 アプリへのサインインに関する問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579870"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="30fc2-102">Microsoft 365 アプリでの「このコンピューターのトラステッド プラットフォーム モジュールが正常に機能していません」というメッセージを解決する</span><span class="sxs-lookup"><span data-stu-id="30fc2-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="30fc2-103">このエラーを解決するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="30fc2-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="30fc2-104">[Windows](https://support.microsoft.com/help/4027667/windows-10-update) および [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5) の最新の更新プログラムをインストールします。</span><span class="sxs-lookup"><span data-stu-id="30fc2-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="30fc2-105">Windows 資格情報マネージャーを使用して、[Office の資格情報をクリア](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)します。</span><span class="sxs-lookup"><span data-stu-id="30fc2-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="30fc2-106">**注:** Office 2016 のレジストリ パスは 16.0 に変更されています。</span><span class="sxs-lookup"><span data-stu-id="30fc2-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="30fc2-107">(例: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="30fc2-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="30fc2-108">[ユーザー回復プロセス](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2)を実行して、トラステッド プラットフォーム モジュール (TPM) の障害の解決を試みてください。</span><span class="sxs-lookup"><span data-stu-id="30fc2-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="30fc2-109">次の手順に従い、EnableADAL = 0 に設定します。</span><span class="sxs-lookup"><span data-stu-id="30fc2-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="30fc2-110">Windows の [スタート] ボタンを右クリックし、[**ファイル名を指定して実行**] を選択します。"**regedit**" と入力し、[**OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="30fc2-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="30fc2-111">[**はい**] を選択して、レジストリ エディターがデバイスに変更を加えることを許可します。</span><span class="sxs-lookup"><span data-stu-id="30fc2-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="30fc2-112">レジストリ エディターで、HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity に **EnableADAL** の DWORD 値を **0** に設定して追加します。</span><span class="sxs-lookup"><span data-stu-id="30fc2-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="30fc2-113">詳細については、「[Windows 10 の Office 2016 ビルド16.0.7967 に更新後のサインインにおける接続の問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30fc2-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>
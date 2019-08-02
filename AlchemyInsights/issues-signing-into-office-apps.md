---
title: Office アプリへのサインインの問題
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
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "36051956"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="a7926-102">Office アプリを修正する "コンピューターのトラステッドプラットフォームモジュールが正しく機能していません。" というメッセージが表示される</span><span class="sxs-lookup"><span data-stu-id="a7926-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="a7926-103">このエラーを解決するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="a7926-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="a7926-104">[Windows](https://support.microsoft.com/help/4027667/windows-10-update)および[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)の最新の更新プログラムをインストールします。</span><span class="sxs-lookup"><span data-stu-id="a7926-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="a7926-105">Windows 資格情報マネージャーを使用して[Office 資格情報をクリア](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)します。</span><span class="sxs-lookup"><span data-stu-id="a7926-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="a7926-106">**注:** Office 2016 のレジストリパスは16.0 に変更されました。</span><span class="sxs-lookup"><span data-stu-id="a7926-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a7926-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="a7926-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="a7926-108">[ユーザー回復プロセス](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2)を試行して、トラステッドプラットフォームモジュール (TPM) の障害を修正します。</span><span class="sxs-lookup"><span data-stu-id="a7926-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="a7926-109">次の手順を使用して、EnableADAL = 0 を設定します。</span><span class="sxs-lookup"><span data-stu-id="a7926-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="a7926-110">Windows の [スタート] ボタンを右クリックし、[**実行**] を選択し、「 **regedit**」と入力して、[ **OK]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a7926-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="a7926-111">[**はい]** を選択して、レジストリエディターでデバイスを変更できるようにします。</span><span class="sxs-lookup"><span data-stu-id="a7926-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="a7926-112">レジストリエディターで、HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity. の下に**0**の設定を使用して**EnableADAL**の DWORD 値を追加します。</span><span class="sxs-lookup"><span data-stu-id="a7926-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="a7926-113">詳細については、「 [Windows 10 の Office 2016 ビルド16.0.7967 での更新後のサインインの接続の問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7926-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>
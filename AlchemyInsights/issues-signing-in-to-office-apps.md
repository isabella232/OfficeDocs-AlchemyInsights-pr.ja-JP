---
title: Office アプリへのサインインに関する問題
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
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "36051953"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="d1ee9-102">Office アプリでの「申し訳ございません。このコンピューターに、組織内の別のアカウントが既にサインインしています」というメッセージを解決する</span><span class="sxs-lookup"><span data-stu-id="d1ee9-102">Fixing the Office apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="d1ee9-103">このエラーを解決するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="d1ee9-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="d1ee9-104">影響を受けているアカウント以外のすべての職場のアカウントを削除します。これを行うには、[Windows の設定] > [**職場または学校にアクセスする**] に移動します。</span><span class="sxs-lookup"><span data-stu-id="d1ee9-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="d1ee9-105">Windows 資格情報マネージャーを使用して、[Office の資格情報をクリア](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)します。</span><span class="sxs-lookup"><span data-stu-id="d1ee9-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d1ee9-106">**注:** Office 2016 のレジストリ パスは 16.0 に変更されています。</span><span class="sxs-lookup"><span data-stu-id="d1ee9-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d1ee9-107">(例: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d1ee9-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="d1ee9-108">Office アプリを開き、[**ファイル**]  >  [**アカウント**]  >  [**サインアウト**] を選択します。その後、有効なライセンスがあるユーザー アカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="d1ee9-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="d1ee9-109">詳細については、「[Office のアカウント](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1ee9-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="d1ee9-110">Mac の場合は、「[Office 2016 for Mac アプリにサインインできない](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1ee9-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="d1ee9-111">詳細については、Office での「[申し訳ございません。このコンピューターに、組織内の別のアカウントが既にサインインしています](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1ee9-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>
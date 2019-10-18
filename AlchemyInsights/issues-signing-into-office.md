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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "36051954"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="19b42-102">Office アプリへのサインインに関する問題</span><span class="sxs-lookup"><span data-stu-id="19b42-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="19b42-103">Officeアプリでのサインインの問題を修正するには、次の操作を試してください。</span><span class="sxs-lookup"><span data-stu-id="19b42-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="19b42-104">影響を受けているアカウント以外のすべての職場のアカウントを削除します。これを行うには、[Windows の設定] > [**職場または学校にアクセスする**] に移動します。</span><span class="sxs-lookup"><span data-stu-id="19b42-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="19b42-105">Windows 資格情報マネージャーを使用して、[Office の資格情報をクリア](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)します。</span><span class="sxs-lookup"><span data-stu-id="19b42-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="19b42-106">**注:** Office 2016 のレジストリ パスは 16.0 に変更されています。</span><span class="sxs-lookup"><span data-stu-id="19b42-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="19b42-107">(例: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="19b42-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="19b42-108">Office アプリを開き、[**ファイル**]  >  [**アカウント**]  >  [**サインアウト**] を選択します。その後、有効なライセンスがあるユーザー アカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="19b42-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="19b42-109">詳細については、「[Office のアカウント](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19b42-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="19b42-110">Mac の場合は、「[Office 2016 for Mac アプリにサインインできない](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19b42-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="19b42-111">Office 2013 を使用し Office 365 へと接続する際にエラーが発生した場合、Office クライアントの先進認証を有効にします。</span><span class="sxs-lookup"><span data-stu-id="19b42-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="19b42-112">詳細については、次のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="19b42-112">For more information, see:</span></span>
- <span data-ttu-id="19b42-113">「[Office 365、Azure、または Intune にサインインできない](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)」</span><span class="sxs-lookup"><span data-stu-id="19b42-113">[You can't sign in to Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)</span></span>
- <span data-ttu-id="19b42-114">「[Windows 10 の Office 2016 ビルド16.0.7967 に更新後のサインインにおける接続の問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)」</span><span class="sxs-lookup"><span data-stu-id="19b42-114">[Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span></span>
- <span data-ttu-id="19b42-115">「[Office での "申し訳ございません。このコンピューターに、組織内の別のアカウントが既にサインインしています"](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)」</span><span class="sxs-lookup"><span data-stu-id="19b42-115">["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span></span>
- <span data-ttu-id="19b42-116">「[ADFS を使用している場合の Office 先進認証によるサインイン問題のトラブルシューティング](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)」</span><span class="sxs-lookup"><span data-stu-id="19b42-116">[How to troubleshoot sign-in issues with Office 2013 modern authentication when you use AD FS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)</span></span>
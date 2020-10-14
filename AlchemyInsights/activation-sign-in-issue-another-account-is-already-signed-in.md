---
title: ライセンス認証/サインインの問題 - 別のアカウントがすでにサインインしている
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3407"
- "9001422"
ms.openlocfilehash: 28cab94af5c3e57bce5a41d36c20a57ebfa825ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697742"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="55989-102">Microsoft 365 アプリでの「申し訳ございません。このコンピューターに、組織内の別のアカウントが既にサインインしています」というメッセージを解決する</span><span class="sxs-lookup"><span data-stu-id="55989-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="55989-103">このエラーを解決するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="55989-103">To fix this error, try the following:</span></span>

1. <span data-ttu-id="55989-104">Office アプリを開き、すべての既存のユーザー アカウントから[サインアウト](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)します。</span><span class="sxs-lookup"><span data-stu-id="55989-104">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>   
2. <span data-ttu-id="55989-105">Windows を使用して [**設定**] > [**アカウント**] > [**メールとアカウント**] の順に移動し、影響を受けるアカウントを除くすべてのアカウントを削除します。</span><span class="sxs-lookup"><span data-stu-id="55989-105">Using Windows **Settings** > **Accounts** > **Email & accounts**, remove all work accounts except the affected account.</span></span> 
3. <span data-ttu-id="55989-106">Windows を使用して [**設定**] > [**アカウント**] > [**職場または学校にアクセスする**] の順に移動し、影響を受けるアカウントを除くすべての職場アカウントを切断します。</span><span class="sxs-lookup"><span data-stu-id="55989-106">Using Windows **Settings** > **Accounts** > **Access work or school**, disconnect all work accounts except the affected account.</span></span> 
4. <span data-ttu-id="55989-107">Office のライセンス認証の状態を再設定します。</span><span class="sxs-lookup"><span data-stu-id="55989-107">Reset Office activation state.</span></span> <span data-ttu-id="55989-108">[詳細情報](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55989-108">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).</span></span>
5. <span data-ttu-id="55989-109">影響を受けるアカウントを使用して[サインイン](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) します。</span><span class="sxs-lookup"><span data-stu-id="55989-109">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span> 

<span data-ttu-id="55989-110">詳細については、「[Office 2013 では、組織の別のアカウントがこのコンピューターで既にサインインしています](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55989-110">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office 2013](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>

<span data-ttu-id="55989-111">Mac の場合は、「[Office 2016 for Mac アプリにサインインできない](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55989-111">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
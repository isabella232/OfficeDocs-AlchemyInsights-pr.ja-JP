---
title: ライセンス認証/サインインの問題 - 別のアカウントがすでにサインインしている
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3407"
- "9001422"
ms.openlocfilehash: 76eef6f89cc1cb4c26e9022c7048d23937e5af59
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822928"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="3012c-102">Microsoft 365 アプリでの「申し訳ございません。このコンピューターに、組織内の別のアカウントが既にサインインしています」というメッセージを解決する</span><span class="sxs-lookup"><span data-stu-id="3012c-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="3012c-103">このエラーを解決するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="3012c-103">To fix this error, try the following:</span></span>

1. <span data-ttu-id="3012c-104">Office アプリを開き、すべての既存のユーザー アカウントから[サインアウト](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)します。</span><span class="sxs-lookup"><span data-stu-id="3012c-104">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>   
2. <span data-ttu-id="3012c-105">Windows を使用して [**設定**] > [**アカウント**] > [**メールとアカウント**] の順に移動し、影響を受けるアカウントを除くすべてのアカウントを削除します。</span><span class="sxs-lookup"><span data-stu-id="3012c-105">Using Windows **Settings** > **Accounts** > **Email & accounts**, remove all work accounts except the affected account.</span></span> 
3. <span data-ttu-id="3012c-106">Windows を使用して [**設定**] > [**アカウント**] > [**職場または学校にアクセスする**] の順に移動し、影響を受けるアカウントを除くすべての職場アカウントを切断します。</span><span class="sxs-lookup"><span data-stu-id="3012c-106">Using Windows **Settings** > **Accounts** > **Access work or school**, disconnect all work accounts except the affected account.</span></span> 
4. <span data-ttu-id="3012c-107">Office のライセンス認証の状態を再設定します。</span><span class="sxs-lookup"><span data-stu-id="3012c-107">Reset Office activation state.</span></span> <span data-ttu-id="3012c-108">[詳細情報](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3012c-108">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).</span></span>
5. <span data-ttu-id="3012c-109">影響を受けるアカウントを使用して[サインイン](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) します。</span><span class="sxs-lookup"><span data-stu-id="3012c-109">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span> 

<span data-ttu-id="3012c-110">詳細については、「[Office 2013 では、組織の別のアカウントがこのコンピューターで既にサインインしています](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3012c-110">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office 2013](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>

<span data-ttu-id="3012c-111">Mac の場合は、「[Office 2016 for Mac アプリにサインインできない](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3012c-111">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
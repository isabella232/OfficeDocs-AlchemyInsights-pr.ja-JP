---
title: ライセンスの認証/サインインの問題 - トラステッド プラットフォーム モジュールの誤動作
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3406"
- "9001429"
ms.openlocfilehash: d1c25bb283def13524b1dcd19d0c746ee32c4e11
ms.sourcegitcommit: efdde3c24a0c1adfb8b6f5f59dcae435fb5c53a8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/19/2019
ms.locfileid: "38749429"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="fd80c-102">Office アプリでの「このコンピューターのトラステッド プラットフォーム モジュールが正常に機能していません 」というメッセージを解決する</span><span class="sxs-lookup"><span data-stu-id="fd80c-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="fd80c-103">このエラーを解決するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="fd80c-103">To fix this error, try the following:</span></span>

1. <span data-ttu-id="fd80c-104">Office アプリを開き、すべての既存のユーザー アカウントから[サインアウト](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)します。</span><span class="sxs-lookup"><span data-stu-id="fd80c-104">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>   
2. <span data-ttu-id="fd80c-105">Windows を使用して [**設定**] > [**アカウント**] > [**メールとアカウント**] の順に移動し、既存の職場のアカウントを削除します。</span><span class="sxs-lookup"><span data-stu-id="fd80c-105">Using Windows **Settings** > **Accounts** > **Email & accounts**, remove all work accounts except the affected account.</span></span> 
3. <span data-ttu-id="fd80c-106">Windows を使用して [**設定**] > [**アカウント**] > [**職場または学校にアクセスする**] の順に移動し、既存のアカウントを切断します。</span><span class="sxs-lookup"><span data-stu-id="fd80c-106">Using Windows **Settings** > **Accounts** > **Access work or school**, disconnect all work accounts except the affected account.</span></span> 
4. <span data-ttu-id="fd80c-107">Office のライセンス認証の状態を再設定します。</span><span class="sxs-lookup"><span data-stu-id="fd80c-107">Reset Office activation state.</span></span> <span data-ttu-id="fd80c-108">[詳細情報](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd80c-108">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).</span></span>
5. <span data-ttu-id="fd80c-109">[ユーザー回復プロセス](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2)を実行して、トラステッド プラットフォーム モジュール (TPM) の障害の解決を試みてください。</span><span class="sxs-lookup"><span data-stu-id="fd80c-109">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
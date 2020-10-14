---
title: ライセンスの認証/サインインの問題 - トラステッド プラットフォーム モジュールの誤動作
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
- "3406"
- "9001429"
ms.openlocfilehash: 13e6fcd18047e511452f0180dc2e4677466d4db3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697526"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="b1c06-102">Microsoft 365 アプリでの「このコンピューターのトラステッド プラットフォーム モジュールが正常に機能していません」というメッセージを解決する</span><span class="sxs-lookup"><span data-stu-id="b1c06-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="b1c06-103">このエラーを解決するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="b1c06-103">To fix this error, try the following:</span></span>

1. <span data-ttu-id="b1c06-104">Office アプリを開き、すべての既存のユーザー アカウントから[サインアウト](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)します。</span><span class="sxs-lookup"><span data-stu-id="b1c06-104">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>   
2. <span data-ttu-id="b1c06-105">Windows を使用して [**設定**] > [**アカウント**] > [**メールとアカウント**] の順に移動し、既存の職場のアカウントを削除します。</span><span class="sxs-lookup"><span data-stu-id="b1c06-105">Using Windows **Settings** > **Accounts** > **Email & accounts**, remove existing work accounts.</span></span> 
3. <span data-ttu-id="b1c06-106">Windows を使用して [**設定**] > [**アカウント**] > [**職場または学校にアクセスする**] の順に移動し、既存のアカウントを切断します。</span><span class="sxs-lookup"><span data-stu-id="b1c06-106">Using Windows **Settings** > **Accounts** > **Access work or school**, disconnect existing accounts.</span></span> 
4. <span data-ttu-id="b1c06-107">Office のライセンス認証の状態を再設定します。</span><span class="sxs-lookup"><span data-stu-id="b1c06-107">Reset Office activation state.</span></span> <span data-ttu-id="b1c06-108">[詳細情報](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1c06-108">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).</span></span>
5. <span data-ttu-id="b1c06-109">[ユーザー回復プロセス](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2)を実行して、トラステッド プラットフォーム モジュール (TPM) の障害の解決を試みてください。</span><span class="sxs-lookup"><span data-stu-id="b1c06-109">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
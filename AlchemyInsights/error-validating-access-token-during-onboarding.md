---
title: Desktop Analytics のオンボーディング中にアクセス トークン エラーを検証する際にエラーが発生しました
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2019
ms.locfileid: "40791279"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="6d870-102">「Desktop Analytics のオンボーディング中にアクセス トークン エラーを検証する際にエラーが発生しました</span><span class="sxs-lookup"><span data-stu-id="6d870-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="6d870-103">このエラーは通常、認証トークンの有効期限が切れたときに発生します。</span><span class="sxs-lookup"><span data-stu-id="6d870-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="6d870-104">通常、ページを更新すると、トークンが更新されます。</span><span class="sxs-lookup"><span data-stu-id="6d870-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="6d870-105">ただし、オンボードの Desktop Analytics で使用されているアカウントに条件付きアクセス ポリシーを適用しても、この問題は解決しません。</span><span class="sxs-lookup"><span data-stu-id="6d870-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="6d870-106">Azure ポータルの Azure AD サインイン ログを確認して、Desktop Analytics のオンボーディングに使用されているアカウントにサインイン エラーがないかどうかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="6d870-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="6d870-107">条件付きアクセスの詳細については、「[条件付きアクセスの展開を計画する](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d870-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>
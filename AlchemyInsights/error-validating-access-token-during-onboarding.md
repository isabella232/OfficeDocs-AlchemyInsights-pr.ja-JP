---
title: デスクトップ分析の実行中にアクセストークンエラーの検証中にエラーが発生しました
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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2019
ms.locfileid: "40791279"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="fc1f2-102">デスクトップ分析のオンボード時に発生する "アクセストークンの検証エラーです" エラー</span><span class="sxs-lookup"><span data-stu-id="fc1f2-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="fc1f2-103">このエラーは、通常、認証トークンの有効期限が切れたときに確認されます。</span><span class="sxs-lookup"><span data-stu-id="fc1f2-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="fc1f2-104">通常、ページを更新すると、トークンが更新されます。</span><span class="sxs-lookup"><span data-stu-id="fc1f2-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="fc1f2-105">ただし、オンボードデスクトップ分析に使用されているアカウントに適用されている条件付きアクセスポリシーがある場合、この問題は引き続き発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="fc1f2-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="fc1f2-106">Azure ポータルの Azure AD サインインログを確認して、デスクトップ分析のオンボードで使用されているアカウントにサインイン失敗があるかどうかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="fc1f2-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="fc1f2-107">条件付きアクセスの詳細については、「[条件付きアクセスの展開を計画する](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc1f2-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>
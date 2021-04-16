---
title: Desktop Analytics のオンボーディング中にアクセス トークン エラーを検証する際にエラーが発生しました
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813693"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>「Desktop Analytics のオンボーディング中にアクセス トークン エラーを検証する際にエラーが発生しました

このエラーは通常、認証トークンの有効期限が切れたときに発生します。 通常、ページを更新すると、トークンが更新されます。 ただし、オンボードの Desktop Analytics で使用されているアカウントに条件付きアクセス ポリシーを適用しても、この問題は解決しません。 Azure ポータルの Azure AD サインイン ログを確認して、Desktop Analytics のオンボーディングに使用されているアカウントにサインイン エラーがないかどうかを確認できます。

条件付きアクセスの詳細については、「[条件付きアクセスの展開を計画する](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)」を参照してください。
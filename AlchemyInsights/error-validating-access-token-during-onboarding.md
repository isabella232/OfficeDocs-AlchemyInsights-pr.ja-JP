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
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>「Desktop Analytics のオンボーディング中にアクセス トークン エラーを検証する際にエラーが発生しました

このエラーは通常、認証トークンの有効期限が切れたときに発生します。 通常、ページを更新すると、トークンが更新されます。 ただし、オンボードの Desktop Analytics で使用されているアカウントに条件付きアクセス ポリシーを適用しても、この問題は解決しません。 Azure ポータルの Azure AD サインイン ログを確認して、Desktop Analytics のオンボーディングに使用されているアカウントにサインイン エラーがないかどうかを確認できます。

条件付きアクセスの詳細については、「[条件付きアクセスの展開を計画する](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)」を参照してください。
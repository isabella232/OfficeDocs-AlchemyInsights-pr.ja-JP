---
title: ユーザーの同意のトラブルシューティング
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007903"
---
# <a name="troubleshoot-user-consent"></a>ユーザーの同意のトラブルシューティング

1. エンドユーザーが Azure Portal または PowerShell を介してアプリケーションに同意する方法を構成できます。 詳細については、「[ユーザーの同意の設定](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings)」をご覧ください。
1. 管理者は、[Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) を使用して、単一のユーザーに代わって委任されたアクセス許可に同意を与えることもできます。 詳細については、「[ユーザーの代わりにアクセスを取得](https://docs.microsoft.com/graph/auth-v2-user)」をご覧ください。
1. [ユーザー同意エラー](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): この記事では、アプリケーションへの同意プロセス中に発生する可能性のあるエラーについて説明します。 エラー メッセージが含まれていない、予期しない同意プロンプトのトラブルシューティングを行う場合は、「[Azure ADの認証シナリオ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)」を参照してください。
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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901745"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="9ac85-102">ユーザーの同意のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="9ac85-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="9ac85-103">エンドユーザーが Azure Portal または PowerShell を介してアプリケーションに同意する方法を構成できます。</span><span class="sxs-lookup"><span data-stu-id="9ac85-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="9ac85-104">詳細については、「[ユーザーの同意の設定](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9ac85-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="9ac85-105">管理者は、[Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) を使用して、単一のユーザーに代わって委任されたアクセス許可に同意を与えることもできます。</span><span class="sxs-lookup"><span data-stu-id="9ac85-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="9ac85-106">詳細については、「[ユーザーの代わりにアクセスを取得](https://docs.microsoft.com/graph/auth-v2-user)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9ac85-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="9ac85-107">[ユーザー同意エラー](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): この記事では、アプリケーションへの同意プロセス中に発生する可能性のあるエラーについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9ac85-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="9ac85-108">エラー メッセージが含まれていない、予期しない同意プロンプトのトラブルシューティングを行う場合は、「[Azure ADの認証シナリオ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ac85-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>
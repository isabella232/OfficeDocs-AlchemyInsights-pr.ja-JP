---
title: アプリ登録クライアントの秘密または証明書の問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405816"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="e4930-102">アプリ登録クライアントの秘密または証明書の問題</span><span class="sxs-lookup"><span data-stu-id="e4930-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="e4930-103">アプリケーション クライアント シークレットの有効期限が切れていますか?</span><span class="sxs-lookup"><span data-stu-id="e4930-103">Application client secret expiring?</span></span>

<span data-ttu-id="e4930-104">登録されたアプリケーションがどのように作成されたかに関係なく、アプリ登録ポータルでの標準の登録プロセスを通じて、またはアプリケーションの同意を使用してサービス プリンシパルがテナントで作成されたかどうかに関係なく、新しいクライアント シークレットは、現在のクライアント シークレットの有効期限が切れる前に作成し、関連するアプリケーション コードで更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4930-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="e4930-105">最大有効期間は 2 年です。</span><span class="sxs-lookup"><span data-stu-id="e4930-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="e4930-106">ポータルのアプリ登録ページを離れると表示されなくなるため、シークレット値を記録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4930-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="e4930-107">詳細については、「[クイックスタート: Microsoft ID プラットフォームへのアプリの登録](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app)」および「[Microsoft ID プラットフォームのベスト プラクティス](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4930-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="e4930-108">詳細については、「[ポータルでの Azure AD アプリとサービス プリンシパルの作成 - Microsoft ID プラットフォーム](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4930-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>

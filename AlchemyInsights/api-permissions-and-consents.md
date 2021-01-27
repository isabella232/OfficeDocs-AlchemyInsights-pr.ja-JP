---
title: API アクセス許可と同意
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975113"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="9c8fa-102">API アクセス許可と同意</span><span class="sxs-lookup"><span data-stu-id="9c8fa-102">API permissions and consent</span></span>

<span data-ttu-id="9c8fa-103">Microsoft ID プラットフォームと統合するアプリケーションは、ユーザーと管理者がデータへのアクセス方法を制御できる承認モデルに従います。</span><span class="sxs-lookup"><span data-stu-id="9c8fa-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="9c8fa-104">承認モデルの実装は、Microsoft ID プラットフォーム エンドポイントで更新されています。</span><span class="sxs-lookup"><span data-stu-id="9c8fa-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="9c8fa-105">これにより、アプリが Microsoft ID プラットフォームを操作する方法が変更されます。</span><span class="sxs-lookup"><span data-stu-id="9c8fa-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="9c8fa-106">「[Microsoft ID プラットフォーム エンドポイントのアクセス許可と同意](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)」は、スコープ、アクセス許可、同意など、この承認モデルの基本的な概念を網羅しています。</span><span class="sxs-lookup"><span data-stu-id="9c8fa-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="9c8fa-107">[Azure Active Directory (Azure AD) 同意フレームワーク](https://docs.microsoft.com/azure/active-directory/develop/consent-framework)を使用すると、マルチテナント Web およびネイティブ クライアント アプリケーションを簡単に開発できます。</span><span class="sxs-lookup"><span data-stu-id="9c8fa-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="9c8fa-108">これらのアプリケーションでは、アプリケーションが登録されているものとは異なる Azure AD テナントからのユーザー アカウントによるサインインが可能です。</span><span class="sxs-lookup"><span data-stu-id="9c8fa-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="9c8fa-109">また、独自の Web API に加えて、Microsoft Graph API (Azure AD、Intune、および Microsoft 365 のサービスにアクセスするため) やその他の Microsoft サービスの API などの Web API にアクセスする必要がある場合もあります。</span><span class="sxs-lookup"><span data-stu-id="9c8fa-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>


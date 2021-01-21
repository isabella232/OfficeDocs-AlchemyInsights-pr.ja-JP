---
title: サインアウトの問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901719"
---
# <a name="sign-out-issues"></a><span data-ttu-id="534ea-102">サインアウトの問題</span><span class="sxs-lookup"><span data-stu-id="534ea-102">Sign-out issues</span></span>

<span data-ttu-id="534ea-103">サインアウトに関連する問題を解決するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="534ea-103">To resolve issues related to signing out, perform the following steps:</span></span>

1. <span data-ttu-id="534ea-104">あなたまたはユーザーがログに記録されたり、アプリケーションから追い出されたりする場合は、記事「[条件付きアクセスを使用して認証セッション管理を構成する](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime)」または「[Microsoft ID プラットフォームでの構成可能なトークンの有効期間](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」のガイダンスに従ってください。</span><span class="sxs-lookup"><span data-stu-id="534ea-104">If you or a user are getting logged or kicked out of applications, follow the guidance in the articles [Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) or [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
2. <span data-ttu-id="534ea-105">他のほとんどのサインアウト エラーまたは問題は、Azure Active Directory (Azure AD) と特定のアプリケーションの統合のトラブルシューティングを行うことで解決できます。</span><span class="sxs-lookup"><span data-stu-id="534ea-105">Most other sign-out errors or problems can be solved by troubleshooting the integration of Azure Active Directory (Azure AD) with the specific application.</span></span> <span data-ttu-id="534ea-106">以下を含む、[アプリケーションを Azure Active Directory と統合するためのチュートリアルのコレクション](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)にアクセスすると、特定の統合に関するガイダンスを見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="534ea-106">You can find guidance for a specific integration by going to this [collection of tutorials for integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), including:</span></span>
    - <span data-ttu-id="534ea-107">SaaS アプリケーションのチュートリアル</span><span class="sxs-lookup"><span data-stu-id="534ea-107">SaaS application tutorials</span></span>
    - <span data-ttu-id="534ea-108">シングル サインオンのチュートリアル</span><span class="sxs-lookup"><span data-stu-id="534ea-108">Single sign-on tutorials</span></span>
    - <span data-ttu-id="534ea-109">ユーザー プロビジョニングのチュートリアル</span><span class="sxs-lookup"><span data-stu-id="534ea-109">User-provisioning tutorials</span></span>
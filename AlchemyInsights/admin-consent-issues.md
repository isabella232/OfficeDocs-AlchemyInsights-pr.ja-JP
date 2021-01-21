---
title: 管理者の同意の問題
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
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901736"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="6c3a0-102">管理者の同意の問題</span><span class="sxs-lookup"><span data-stu-id="6c3a0-102">Admin consent issues</span></span>

1. <span data-ttu-id="6c3a0-103">[管理者同意ワークフロー](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow)を有効にして、ユーザーが同意画面から直接管理者の承認を要求できるようにします。</span><span class="sxs-lookup"><span data-stu-id="6c3a0-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="6c3a0-104">同意プロセス中にあなたまたはアプリケーションのユーザーに予期しないエラーが表示される場合は、トラブルシューティング手順について次の記事を参照してください：[「アプリケーションに同意すると、予期しないエラーが発生する」](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)。</span><span class="sxs-lookup"><span data-stu-id="6c3a0-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="6c3a0-105">[Microsoft ID プラットフォームでの管理者の同意](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)、[同意プロンプト](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)の仕組み、および[テナント全体の管理者の同意の要求を評価する](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)方法の詳細をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6c3a0-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="6c3a0-106">Microsoft ID プラットフォームと統合するアプリケーションは、ユーザーと管理者がデータへのアクセス方法を制御できる承認モデルに従います。</span><span class="sxs-lookup"><span data-stu-id="6c3a0-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="6c3a0-107">承認モデルの実装は、Microsoft ID プラットフォームエンドポイントで更新され、それにより、アプリが Microsoft ID プラットフォームと対話する方法が変更されました。</span><span class="sxs-lookup"><span data-stu-id="6c3a0-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="6c3a0-108">スコープ、アクセス許可、同意など、この承認モデルの概要については、「[Microsoft ID プラットフォーム エンドポイントのアクセス許可と同意](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c3a0-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>
---
title: トークンの有効期限の構成と延長
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917277"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="e52c4-102">トークンの有効期限の構成と延長</span><span class="sxs-lookup"><span data-stu-id="e52c4-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="e52c4-103">Microsoft ID プラットフォームによって発行されるアクセス、SAML、または ID トークンの有効期限を指定できます。</span><span class="sxs-lookup"><span data-stu-id="e52c4-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="e52c4-104">組織のすべてのアプリ、マルチテナント (多組織) アプリケーション、組織の特定のサービス プリンシパルにトークンの有効期間を設定できます。</span><span class="sxs-lookup"><span data-stu-id="e52c4-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="e52c4-105">詳細については、「[構成可能なトークンの有効期限](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e52c4-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="e52c4-106">たとえば、「[トークンの有効期限の構成例](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e52c4-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="e52c4-107">Azure Active Directory B2C (Azure AD B2C) のトークンの有効期限と互換性を構成する方法については、「[Azure Active Directory B2C でトークンを構成する](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e52c4-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="e52c4-108">記事「[Azure Active Directory B2C でのセッション動作を構成する](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow)」では、Azure AD B2C で使用されるシングル サインオン (SSO) 方式について説明し、ポリシーを構成するときに最適な SSO 方式を選択するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="e52c4-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="e52c4-109">**トークンの有効期間はどのぐらいですか?いつまで有効ですか?**</span><span class="sxs-lookup"><span data-stu-id="e52c4-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="e52c4-110">トークンの有効期限は 1 時間、セッションの有効期限は 24 時間です。</span><span class="sxs-lookup"><span data-stu-id="e52c4-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="e52c4-111">つまり、24 時間以内に要求が行われなかった場合は、新しいトークンを要求する前に再度ログインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="e52c4-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="e52c4-112">2020 年 5 月 30 日を過ぎると、新しいテナントは構成可能なトークンの有効期間ポリシーを使用してセッションおよびトークンの更新を構成できなくなります。</span><span class="sxs-lookup"><span data-stu-id="e52c4-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="e52c4-113">その後数ヶ月以内に廃止されるため、既存のセッションの承認を停止し、トークン ポリシーを更新します。</span><span class="sxs-lookup"><span data-stu-id="e52c4-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="e52c4-114">廃止された後も、アクセス トークンの有効期限を構成できます。</span><span class="sxs-lookup"><span data-stu-id="e52c4-114">You can still configure access token lifetimes after the deprecation.</span></span>







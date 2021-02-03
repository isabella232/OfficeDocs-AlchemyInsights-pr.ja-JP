---
title: 認証ライブラリに関する問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063730"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="0dd64-102">認証ライブラリに関する問題</span><span class="sxs-lookup"><span data-stu-id="0dd64-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="0dd64-103">[Microsoft ID プラットフォーム認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)には、Microsoft がサポートする互換性のあるクライアントおよびミドルウェア ライブラリが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="0dd64-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="0dd64-104">Microsoft Authentication Library (MSAL) は、さまざまなアプリケーション シナリオで使用する複数の[認証フロー](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows)をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="0dd64-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="0dd64-105">トークンを認証して取得するには、コードで新しいパブリックまたは機密のクライアント アプリケーションを初期化します。</span><span class="sxs-lookup"><span data-stu-id="0dd64-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="0dd64-106">Microsoft Authentication Library (MSAL) でクライアント アプリを初期化するときに、いくつかの構成オプションを設定できます。</span><span class="sxs-lookup"><span data-stu-id="0dd64-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="0dd64-107">詳細については、「[アプリケーション構成オプション](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0dd64-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="0dd64-108">**Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) のサポートの終了** _</span><span class="sxs-lookup"><span data-stu-id="0dd64-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="0dd64-109">**2020 年 6 月 30 日以降**、ADAL および Azure AD Graph に新しい機能は追加されなくなります。</span><span class="sxs-lookup"><span data-stu-id="0dd64-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="0dd64-110">テクニカル サポートおよびセキュリティ更新プログラムは引き続き提供されますが、機能の更新プログラムは提供されなくなります。</span><span class="sxs-lookup"><span data-stu-id="0dd64-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="0dd64-111">**2022 年 6月 30 日以降**、ADAL と Azure AD Graph のサポートは終了し、テクニカル サポートやセキュリティ更新プログラムは提供されなくなります。</span><span class="sxs-lookup"><span data-stu-id="0dd64-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="0dd64-112">既存の OS バージョンで ADAL を使用するアプリは、この期間以降も引き続き機能しますが、*テクニカル サポートやセキュリティ更新プログラムの提供* は行われません。</span><span class="sxs-lookup"><span data-stu-id="0dd64-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="0dd64-113">これ以降に Azure AD Graph を使用するアプリは、Azure AD Graph エンドポイントからの応答を受信しなくなる場合があります。</span><span class="sxs-lookup"><span data-stu-id="0dd64-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="0dd64-114">**ADAL 移行**</span><span class="sxs-lookup"><span data-stu-id="0dd64-114">**ADAL Migration**</span></span>

<span data-ttu-id="0dd64-115">最新の機能とセキュリティ更新プログラムを備えた[Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) に更新することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="0dd64-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="0dd64-116">Microsoft アプリを使用している場合は、Microsoft がサポート終了期限までにアプリケーションを MSAL に移行していることを確認し、継続的に MSAL の強化されたセキュリティと機能を利用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="0dd64-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="0dd64-117">詳しくは、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0dd64-117">For more information, see:</span></span>

1. [<span data-ttu-id="0dd64-118">ADAL の FAQ を読む</span><span class="sxs-lookup"><span data-stu-id="0dd64-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="0dd64-119">プラットフォームごとにアプリを移行する方法に関する詳細情報</span><span class="sxs-lookup"><span data-stu-id="0dd64-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="0dd64-120">どのアプリが ADAL を使用しているかを理解するためにサポートが必要な場合は、すべてのアプリのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="0dd64-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="0dd64-121">Microsoft サポートでは、テナントにあるすべての Microsoft ADAL 以外のアプリのリストも提供できます。</span><span class="sxs-lookup"><span data-stu-id="0dd64-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="0dd64-122">**AAD Graph の移行**</span><span class="sxs-lookup"><span data-stu-id="0dd64-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="0dd64-123">Azure AD Graph を使用しているアプリケーションの場合は、ガイダンスに従って [Azure AD Graph アプリを Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview) に移行してください。</span><span class="sxs-lookup"><span data-stu-id="0dd64-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="0dd64-124">[移行のチェックリストは、開始ポイントを提供します](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。</span><span class="sxs-lookup"><span data-stu-id="0dd64-124">[Our migration checklist provides a getting started point.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span></span>
2. <span data-ttu-id="0dd64-125">Azure アプリの登録ポータルには、AAD Graph を使用しているアプリケーションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="0dd64-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="0dd64-126">アプリのすべてのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="0dd64-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="0dd64-127">Microsoft のサポートでは、テナントでのすべての AAD Graph の使用状況のリストを提供することもできます。</span><span class="sxs-lookup"><span data-stu-id="0dd64-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="0dd64-128">アプリから Microsoft Graph のデータにアクセスする場合、ユーザーまたは管理者は、同意のプロセスを通してそのアプリに正しいアクセス許可を付与する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0dd64-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="0dd64-129">[Microsoft Graph のアクセス許可リファレンス](https://docs.microsoft.com/graph/permissions-reference)では、Microsoft Graph API の各主要なセットに関連付けられているアクセス許可について説明します。</span><span class="sxs-lookup"><span data-stu-id="0dd64-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="0dd64-130">また、アクセス許可の使用方法に関するガイダンスを提供しています。</span><span class="sxs-lookup"><span data-stu-id="0dd64-130">It also provides guidance about how to use the permissions.</span></span>

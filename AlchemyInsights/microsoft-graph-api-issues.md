---
title: Microsoft Graph API に関する問題
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/29/2021
ms.locfileid: "50053090"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="07ecc-102">Microsoft Graph API に関する問題</span><span class="sxs-lookup"><span data-stu-id="07ecc-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="07ecc-103">このトピックは、Azure AD Graph API をまだ使用している開発者にも当てはまります。</span><span class="sxs-lookup"><span data-stu-id="07ecc-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="07ecc-104">ただし、すべてのディレクトリ、ID、およびアクセス管理シナリオで Microsoft Graph を使用することを **強く** お勧めします。</span><span class="sxs-lookup"><span data-stu-id="07ecc-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="07ecc-105">**認証または許可に関する問題**</span><span class="sxs-lookup"><span data-stu-id="07ecc-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="07ecc-106">アプリが Microsoft Graph を呼び出すための **トークンを取得できない** 場合、**アクセス トークンの取得に関する問題 (認証)** Microsoft Graph カテゴリを選択して、このトピックに関するより具体的なヘルプとサポートを受けることができます。</span><span class="sxs-lookup"><span data-stu-id="07ecc-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="07ecc-107">Microsoft Graph を呼び出しているときにアプリが **401 または 403 の認証エラー** を受信している場合は、**アクセス拒否エラー (認証)** Microsoft Graph API カテゴリを選択すると、このトピックに関するより具体的なヘルプとサポートを受けることができます。</span><span class="sxs-lookup"><span data-stu-id="07ecc-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="07ecc-108">**Microsoft Graph を使用したいが、開始点がわかりません**</span><span class="sxs-lookup"><span data-stu-id="07ecc-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="07ecc-109">Microsoft Graph の概要</span><span class="sxs-lookup"><span data-stu-id="07ecc-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="07ecc-110">Microsoft Graph の ID およびアクセス管理の概要</span><span class="sxs-lookup"><span data-stu-id="07ecc-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="07ecc-111">Microsoft Graph アプリの作成の開始</span><span class="sxs-lookup"><span data-stu-id="07ecc-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="07ecc-112">**Microsoft Graph エクスプローラー** - テナントまたはデモ テナントで Microsoft Graph API をテストする</span><span class="sxs-lookup"><span data-stu-id="07ecc-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="07ecc-113">**Microsoft Graph を使用したいが、必要な v1.0 ディレクトリ API をサポートしていますか?**</span><span class="sxs-lookup"><span data-stu-id="07ecc-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="07ecc-114">Microsoft Graph は、ディレクトリ、ID、およびアクセス管理に推奨される API です。</span><span class="sxs-lookup"><span data-stu-id="07ecc-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="07ecc-115">しかし、Azure AD Graph と Microsoft Graph にはまだいくつかのギャップがあります。</span><span class="sxs-lookup"><span data-stu-id="07ecc-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="07ecc-116">次の記事を確認してください。これらの記事では、選択に役立つ最新の違いを強調しています。</span><span class="sxs-lookup"><span data-stu-id="07ecc-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="07ecc-117">Azure AD Graph と Microsoft Graph のリソースの種類の違い</span><span class="sxs-lookup"><span data-stu-id="07ecc-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="07ecc-118">Azure AD Graph と Microsoft Graph のプロパティの違い</span><span class="sxs-lookup"><span data-stu-id="07ecc-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="07ecc-119">Azure AD と Microsoft Graph のメソッドの違い</span><span class="sxs-lookup"><span data-stu-id="07ecc-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="07ecc-120">**呼び出している API が機能しません。詳細なテストはどこで実行できますか?**</span><span class="sxs-lookup"><span data-stu-id="07ecc-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="07ecc-121">**Microsoft Graph エクスプローラー** - テナントまたはデモ テナントで Microsoft Graph API をテストし、Microsoft Graph エクスプローラーで **サンプル クエリ** を確認します。</span><span class="sxs-lookup"><span data-stu-id="07ecc-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="07ecc-122">**アプリは遅すぎて、制限されています。改善する方法はありますか?**</span><span class="sxs-lookup"><span data-stu-id="07ecc-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="07ecc-123">シナリオに応じて、アプリケーションのパフォーマンスを向上させ、場合によっては、サービスによって制限される可能性を低くする (呼び出しが多すぎる場合) ために、各種のオプションを自由に使用できます。</span><span class="sxs-lookup"><span data-stu-id="07ecc-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="07ecc-124">Microsoft Graph のベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="07ecc-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="07ecc-125">バッチ要求</span><span class="sxs-lookup"><span data-stu-id="07ecc-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="07ecc-126">デルタ クエリによる変更の追跡</span><span class="sxs-lookup"><span data-stu-id="07ecc-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="07ecc-127">Web フックによる変更の通知を受ける</span><span class="sxs-lookup"><span data-stu-id="07ecc-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="07ecc-128">調整ガイダンス</span><span class="sxs-lookup"><span data-stu-id="07ecc-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="07ecc-129">**エラーおよび既知の問題に関する詳細情報はどこで確認できますか?**</span><span class="sxs-lookup"><span data-stu-id="07ecc-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="07ecc-130">Microsoft Graph のエラー応答情報</span><span class="sxs-lookup"><span data-stu-id="07ecc-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="07ecc-131">Microsoft Graph に関する既知の問題</span><span class="sxs-lookup"><span data-stu-id="07ecc-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="07ecc-132">**サービスの可用性と接続状態はどこで確認できますか?**</span><span class="sxs-lookup"><span data-stu-id="07ecc-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="07ecc-133">Microsoft Graph を介してアクセスできる基礎となるサービスのサービス可用性と接続性は、Microsoft Graph の全体的な可用性とパフォーマンスに影響を与える可能性があります。</span><span class="sxs-lookup"><span data-stu-id="07ecc-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="07ecc-134">Azure Active Directory サービスの正常性については、「[Azure 状態ページ](https://azure.microsoft.com/status/)にリストされている **セキュリティ + ID** サービスの状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="07ecc-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="07ecc-135">Microsoft Graph に貢献する Office サービスについては、「[Office サービス正常性ダッシュボード](https://portal.office.com/adminportal/home#/servicehealth)にリストされているサービスの状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="07ecc-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="07ecc-136">Microsoft Graph の認証エラーは、いくつかの異なる問題の結果である可能性があり、そのほとんどは 401または 403 エラーを生成します。</span><span class="sxs-lookup"><span data-stu-id="07ecc-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="07ecc-137">たとえば、次の場合はすべて承認エラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="07ecc-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="07ecc-138">間違った[アクセス トークンの取得フロー](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="07ecc-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="07ecc-139">十分に構成されていない[アクセス許可スコープ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="07ecc-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="07ecc-140">[同意](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)がない</span><span class="sxs-lookup"><span data-stu-id="07ecc-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="07ecc-141">\**_Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) のサポートの終了_* _</span><span class="sxs-lookup"><span data-stu-id="07ecc-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="07ecc-142">_\*2020 年 6 月 30 日以降\*\*、ADAL および Azure AD Graph に新しい機能は追加されなくなります。</span><span class="sxs-lookup"><span data-stu-id="07ecc-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="07ecc-143">テクニカル サポートおよびセキュリティ更新プログラムは引き続き提供されますが、機能の更新プログラムは提供されなくなります。</span><span class="sxs-lookup"><span data-stu-id="07ecc-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="07ecc-144">**2022 年 6月 30 日以降**、ADAL と Azure AD Graph のサポートは終了し、テクニカル サポートやセキュリティ更新プログラムは提供されなくなります。</span><span class="sxs-lookup"><span data-stu-id="07ecc-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="07ecc-145">既存の OS バージョンで ADAL を使用するアプリは、この期間以降も引き続き機能しますが、*テクニカル サポートやセキュリティ更新プログラムの提供* は行われません。</span><span class="sxs-lookup"><span data-stu-id="07ecc-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="07ecc-146">これ以降に Azure AD Graph を使用するアプリは、Azure AD Graph エンドポイントからの応答を受信しなくなる場合があります。</span><span class="sxs-lookup"><span data-stu-id="07ecc-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="07ecc-147">**ADAL 移行**</span><span class="sxs-lookup"><span data-stu-id="07ecc-147">**ADAL Migration**</span></span>

<span data-ttu-id="07ecc-148">最新の機能とセキュリティ更新プログラムを備えた[Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) に更新することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="07ecc-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="07ecc-149">Microsoft アプリを使用している場合は、Microsoft がサポート終了期限までにアプリケーションを MSAL に移行していることを確認し、継続的に MSAL の強化されたセキュリティと機能を利用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="07ecc-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="07ecc-150">ADAL の FAQ を読む</span><span class="sxs-lookup"><span data-stu-id="07ecc-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="07ecc-151">プラットフォームごとにアプリを移行する方法に関する詳細情報</span><span class="sxs-lookup"><span data-stu-id="07ecc-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="07ecc-152">どのアプリが ADAL を使用しているかを理解するためにサポートが必要な場合は、すべてのアプリのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="07ecc-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="07ecc-153">Microsoft サポートでは、テナントにあるすべての Microsoft ADAL 以外のアプリのリストも提供できます。</span><span class="sxs-lookup"><span data-stu-id="07ecc-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="07ecc-154">**AAD Graph の移行**</span><span class="sxs-lookup"><span data-stu-id="07ecc-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="07ecc-155">Azure AD Graph を使用しているアプリケーションの場合は、ガイダンスに従って [Azure AD Graph アプリを Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview) に移行してください。</span><span class="sxs-lookup"><span data-stu-id="07ecc-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="07ecc-156">[移行のチェックリストは、開始ポイントを提供します](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。</span><span class="sxs-lookup"><span data-stu-id="07ecc-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="07ecc-157">Azure アプリの登録ポータルには、AAD Graph を使用しているアプリケーションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="07ecc-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="07ecc-158">アプリのすべてのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="07ecc-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="07ecc-159">Microsoft のサポートでは、テナントでのすべての AAD Graph の使用状況のリストを提供することもできます。</span><span class="sxs-lookup"><span data-stu-id="07ecc-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="07ecc-160">アプリから Microsoft Graph のデータにアクセスする場合、ユーザーまたは管理者は、同意のプロセスを通してそのアプリに正しいアクセス許可を付与する必要があります。</span><span class="sxs-lookup"><span data-stu-id="07ecc-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="07ecc-161">[Microsoft Graph のアクセス許可リファレンス](https://docs.microsoft.com/graph/permissions-reference)では、Microsoft Graph API の各主要なセットに関連付けられているアクセス許可について説明します。</span><span class="sxs-lookup"><span data-stu-id="07ecc-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="07ecc-162">また、アクセス許可の使用方法に関するガイダンスを提供しています。</span><span class="sxs-lookup"><span data-stu-id="07ecc-162">It also provides guidance about how to use the permissions.</span></span>

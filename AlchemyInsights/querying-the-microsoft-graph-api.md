---
title: Microsoft Graph API のクエリ
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975087"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="a6aad-102">Microsoft Graph API のクエリ</span><span class="sxs-lookup"><span data-stu-id="a6aad-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="a6aad-103">このトピックは、Azure AD Graph API をまだ使用している開発者にも当てはまります。</span><span class="sxs-lookup"><span data-stu-id="a6aad-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="a6aad-104">ただし、すべてのディレクトリ、ID、およびアクセス管理シナリオで Microsoft Graph を使用することを **強く** お勧めします。</span><span class="sxs-lookup"><span data-stu-id="a6aad-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="a6aad-105">**認証または許可に関する問題**</span><span class="sxs-lookup"><span data-stu-id="a6aad-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="a6aad-106">アプリが Microsoft Graph を呼び出すための **トークンを取得できない** 場合、**アクセス トークンの取得に関する問題 (認証)** Microsoft Graph カテゴリを選択して、このトピックに関するより具体的なヘルプとサポートを受けることができます。</span><span class="sxs-lookup"><span data-stu-id="a6aad-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="a6aad-107">Microsoft Graph を呼び出しているときにアプリが **401 または 403 の認証エラー** を受信している場合は、**アクセス拒否エラー (認証)** Microsoft Graph API カテゴリを選択すると、このトピックに関するより具体的なヘルプとサポートを受けることができます。</span><span class="sxs-lookup"><span data-stu-id="a6aad-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="a6aad-108">**Microsoft Graph を使用したいが、開始点がわかりません**</span><span class="sxs-lookup"><span data-stu-id="a6aad-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="a6aad-109">Microsoft Graph の詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6aad-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="a6aad-110">Microsoft Graph の概要</span><span class="sxs-lookup"><span data-stu-id="a6aad-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="a6aad-111">Microsoft Graph の ID およびアクセス管理の概要</span><span class="sxs-lookup"><span data-stu-id="a6aad-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="a6aad-112">Microsoft Graph アプリの作成の開始</span><span class="sxs-lookup"><span data-stu-id="a6aad-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="a6aad-113">**Microsoft Graph エクスプローラー** - テナントまたはデモ テナントで Microsoft Graph API をテストする</span><span class="sxs-lookup"><span data-stu-id="a6aad-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="a6aad-114">**Microsoft Graph を使用したいが、必要な v1.0 ディレクトリ API をサポートしていますか?**</span><span class="sxs-lookup"><span data-stu-id="a6aad-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="a6aad-115">Microsoft Graph は、ディレクトリ、ID、およびアクセス管理に推奨される API です。</span><span class="sxs-lookup"><span data-stu-id="a6aad-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="a6aad-116">しかし、Azure AD Graph と Microsoft Graph にはまだいくつかのギャップがあります。</span><span class="sxs-lookup"><span data-stu-id="a6aad-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="a6aad-117">次の記事を確認してください。これらの記事では、選択に役立つ最新の違いを強調しています。</span><span class="sxs-lookup"><span data-stu-id="a6aad-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="a6aad-118">Azure AD Graph と Microsoft Graph のリソースの種類の違い</span><span class="sxs-lookup"><span data-stu-id="a6aad-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="a6aad-119">Azure AD Graph と Microsoft Graph のプロパティの違い</span><span class="sxs-lookup"><span data-stu-id="a6aad-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="a6aad-120">Azure AD と Microsoft Graph のメソッドの違い</span><span class="sxs-lookup"><span data-stu-id="a6aad-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="a6aad-121">***user* オブジェクトにクエリを実行すると、そのプロパティの多くが欠落します**</span><span class="sxs-lookup"><span data-stu-id="a6aad-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="a6aad-122">Microsoft Graph では *user* プロパティの既定のセットが自動的に選択されるため、`GET https://graph.microsoft.com/v1.0/users` は 11 プロパティだけを返します。</span><span class="sxs-lookup"><span data-stu-id="a6aad-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="a6aad-123">他の *user* プロパティが必要な場合は、$select を使用してアプリケーションに必要なプロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="a6aad-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="a6aad-124">まず **Microsoft Graph エクスプローラー** で試してください。</span><span class="sxs-lookup"><span data-stu-id="a6aad-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="a6aad-125">**一部の user プロパティ値は、設定されていても *null* です**</span><span class="sxs-lookup"><span data-stu-id="a6aad-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="a6aad-126">最も可能性の高い説明は、アプリケーションに *User.ReadBasic.All* アクセス許可が付与されていることです。</span><span class="sxs-lookup"><span data-stu-id="a6aad-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="a6aad-127">これにより、アプリケーションは限られた user プロパティ セットを読み取り、その他すべてのプロパティが以前に設定されていた場合でも null として返されます。</span><span class="sxs-lookup"><span data-stu-id="a6aad-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="a6aad-128">代わりに、アプリケーションに *User.Read.All* アクセス許可を付与してみます。</span><span class="sxs-lookup"><span data-stu-id="a6aad-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="a6aad-129">詳細については、「[Microsoft Graph の user アクセス許可](https://docs.microsoft.com/graph/permissions-reference#user-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6aad-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="a6aad-130">**OData クエリ パラメーターを使用して要求内のデータをフィルター処理できません**</span><span class="sxs-lookup"><span data-stu-id="a6aad-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="a6aad-131">Microsoft Graph は幅広い OData クエリー パラメーターをサポートしていますが、これらのパラメーターの多くは、Microsoft Graph のディレクトリ サービス (*directoryObject* から継承したリソース) では完全にはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6aad-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="a6aad-132">Azure AD Graph と同じ制限事項が Microsoft Graph の大部分で残っています。</span><span class="sxs-lookup"><span data-stu-id="a6aad-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="a6aad-133">**サポートなし**: *null* 値または *not null* 値に対する$count、$search、および $filter</span><span class="sxs-lookup"><span data-stu-id="a6aad-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="a6aad-134">**サポートなし**: 特定のプロパティの $filter on (プロパティがフィルター処理可能なリソースのトピックを参照）</span><span class="sxs-lookup"><span data-stu-id="a6aad-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="a6aad-135">**サポートなし**: ページング、フィルター処理、およびソートを同時に実行</span><span class="sxs-lookup"><span data-stu-id="a6aad-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="a6aad-136">**サポートなし**: 関係に基づくフィルター処理</span><span class="sxs-lookup"><span data-stu-id="a6aad-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="a6aad-137">たとえば、英国にあるすべてのエンジニアリング グループのメンバーを検索します。</span><span class="sxs-lookup"><span data-stu-id="a6aad-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="a6aad-138">**一部サポート**: *user* (displayName と userPrincipalName のみ) と *group* の $orderby</span><span class="sxs-lookup"><span data-stu-id="a6aad-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="a6aad-139">**一部サポート**: $filter (*eq*、*startswith*、*or*、*and* のみサポートし、*any* は制限) サポート、$expand (単一のオブジェクトの関係を展開するとすべての関係が返されるが、オブジェクトの関係のコレクションを展開すると制限あり)</span><span class="sxs-lookup"><span data-stu-id="a6aad-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="a6aad-140">詳細については、「[クエリ パラメーターを使用して応答をカスタマイズする](https://docs.microsoft.com/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6aad-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="a6aad-141">**呼び出している API が機能しません。詳細なテストはどこで実行できますか?**</span><span class="sxs-lookup"><span data-stu-id="a6aad-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="a6aad-142">**Microsoft Graph エクスプローラー** - テナントまたはデモ テナントで Microsoft Graph API をテストし、Microsoft Graph エクスプローラーで **サンプル クエリ** を確認します。</span><span class="sxs-lookup"><span data-stu-id="a6aad-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="a6aad-143">**データをクエリすると、不完全なデータ セットが返されるようです**</span><span class="sxs-lookup"><span data-stu-id="a6aad-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="a6aad-144">コレクションをクエリする場合 (たとえば、*users*)、Microsoft Graph ではサーバー側のページ制限が使用されるため、結果は常に既定のページサイズで返されます。</span><span class="sxs-lookup"><span data-stu-id="a6aad-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="a6aad-145">アプリは常に、サービスから返されたコレクションをページングすることを期待する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6aad-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="a6aad-146">詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6aad-146">For more information, see:</span></span>

- [<span data-ttu-id="a6aad-147">Microsoft Graph のベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="a6aad-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="a6aad-148">アプリの Microsoft Graph データをページングする</span><span class="sxs-lookup"><span data-stu-id="a6aad-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="a6aad-149">**アプリは遅すぎて、制限もされています。改善する方法はありますか?**</span><span class="sxs-lookup"><span data-stu-id="a6aad-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="a6aad-150">シナリオに応じて、アプリケーションのパフォーマンスを向上させ、場合によっては、サービスによって制限される可能性を低くする (呼び出しが多すぎる場合) ために、さまざまなオプションを自由に使用できます。</span><span class="sxs-lookup"><span data-stu-id="a6aad-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="a6aad-151">詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6aad-151">To learn more, see:</span></span>

- [<span data-ttu-id="a6aad-152">Microsoft Graph のベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="a6aad-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="a6aad-153">バッチ要求</span><span class="sxs-lookup"><span data-stu-id="a6aad-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="a6aad-154">デルタ クエリによる変更の追跡</span><span class="sxs-lookup"><span data-stu-id="a6aad-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="a6aad-155">Web フックによる変更の通知を受ける</span><span class="sxs-lookup"><span data-stu-id="a6aad-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="a6aad-156">調整ガイダンス</span><span class="sxs-lookup"><span data-stu-id="a6aad-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="a6aad-157">**エラーおよび既知の問題に関する詳細情報はどこで確認できますか?**</span><span class="sxs-lookup"><span data-stu-id="a6aad-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="a6aad-158">Microsoft Graph のエラー応答情報</span><span class="sxs-lookup"><span data-stu-id="a6aad-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="a6aad-159">Microsoft Graph に関する既知の問題</span><span class="sxs-lookup"><span data-stu-id="a6aad-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="a6aad-160">**サービスの可用性と接続状態はどこで確認できますか?**</span><span class="sxs-lookup"><span data-stu-id="a6aad-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="a6aad-161">Microsoft Graph を介してアクセスできる基礎となるサービスのサービス可用性と接続性は、Microsoft Graph の全体的な可用性とパフォーマンスに影響を与える可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a6aad-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="a6aad-162">Azure Active Directory サービスの正常性については、「[Azure 状態ページ](https://azure.microsoft.com/status/)にリストされている **セキュリティ + ID** サービスの状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="a6aad-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="a6aad-163">Microsoft Graph に貢献する Office サービスについては、「[Office サービス正常性ダッシュボード](https://portal.office.com/adminportal/home#/servicehealth)にリストされているサービスの状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="a6aad-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

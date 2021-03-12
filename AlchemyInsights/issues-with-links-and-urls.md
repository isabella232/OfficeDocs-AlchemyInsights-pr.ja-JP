---
title: リンクおよび URL に関する問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707887"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="cdbb8-102">リンクおよび URL に関する問題</span><span class="sxs-lookup"><span data-stu-id="cdbb8-102">Issues with links and URLs</span></span>

<span data-ttu-id="cdbb8-103">リダイレクト URI/応答 URL (どちらの表現も置き替え可能) は、Microsoft ID プラットフォームがアプリ要求トークンを返すために使用する URL です。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="cdbb8-104">これらの URL の詳細については、以下の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="cdbb8-105">[認証フローとアプリケーション シナリオ](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - 各シナリオの **アプリ登録** ページのリダイレクト URI に関する情報。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="cdbb8-106">リダイレクト URI/応答 URL の制限事項</span><span class="sxs-lookup"><span data-stu-id="cdbb8-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="cdbb8-107">**アプリの正しいリダイレクト URI/応答 URL の登録方法がわかりません**</span><span class="sxs-lookup"><span data-stu-id="cdbb8-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="cdbb8-108">開発中のアプリケーションでサインインするときに、サインイン ダイアログに **AADSTS50011 と表示される場合: 要求で指定された応答 URL がアプリケーション <your app ID>** に構成された応答 URL と一致しません。アプリケーション登録に、Microsoft ID プラットフォームへのトークン要求で使用したコードのリダイレクト URI を追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="cdbb8-109">応答 URL を追加するには、Azure portal の **アプリケーション登録** ページの **[認証]** タブに移動し、**リダイレクト URI** セクションにエントリを追加します。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="cdbb8-110">入力する必要がある値は、次に説明するように、作成するアプリケーションの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-110">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="cdbb8-111">シングルページ アプリケーションおよび Web アプリの場合、応答 URL はアプリケーション内の URL です。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-111">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="cdbb8-112">「[シングルページのアプリケーション登録](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri)」または「[Azure portal を使用した Web アプリの登録](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)」を参照</span><span class="sxs-lookup"><span data-stu-id="cdbb8-112">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="cdbb8-113">デスクトップ アプリの場合、選択する必要がある値は次の条件によって異なります。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-113">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="cdbb8-114">プラットフォーム (MacOS は Windows または Linux とは異なる)</span><span class="sxs-lookup"><span data-stu-id="cdbb8-114">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="cdbb8-115">トークンの取得方法 (対話型でデバイス コード フロー、統合 Windows 認証 [IWA]、またはユーザー名/パスワードを使用)</span><span class="sxs-lookup"><span data-stu-id="cdbb8-115">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="cdbb8-116">詳細については、「[デスクトップ アプリ - アプリ登録 - リダイレクト URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-116">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="cdbb8-117">モバイル アプリケーションの場合、リダイレクト URI は次の条件によって異なります。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-117">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="cdbb8-118">プラットフォーム (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="cdbb8-118">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="cdbb8-119">iOS のバンドル ID、Android のパッケージ名と署名ハッシュなど、アプリを作成するために使用される情報 Azure portal アプリの登録が役立ちます。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-119">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="cdbb8-120">詳細については、「[プラットフォーム構成およびリダイレクト URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-120">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="cdbb8-121">Web API およびトークン取得の一部のサイレント方法 (IWA およびユーザー名/パスワード) には、リダイレクト URI は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-121">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="cdbb8-122">**Web アプリケーションを展開しましたが、展開したアプリをテストすると URL 不一致メッセージが表示されます**</span><span class="sxs-lookup"><span data-stu-id="cdbb8-122">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="cdbb8-123">Web アプリケーションを展開しているすべてのロケーションにリダイレクト URI を追加します。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-123">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="cdbb8-124">詳細については、「[Azure portal を使用して Web アプリを登録する](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-124">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="cdbb8-125">アプリケーションをロケーションに展開した直後に、そのロケーションのリダイレクト URI を追加します。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-125">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="cdbb8-126">**応答 URL を十分に登録できません**</span><span class="sxs-lookup"><span data-stu-id="cdbb8-126">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="cdbb8-127">ISV であり、お客様ごとに 1 つまたは複数のリダイレクト URI があります。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-127">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="cdbb8-128">ADAL/Azure AD v1.0 から MSAL/Microsoft ID プラットフォームに移行する場合、[リダイレクト URI の最大数](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)に達します。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-128">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="cdbb8-129">これを解決するには、お客様ごとに対応する[サービス プリンシパルにリダイレクト URI を追加](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals)します。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-129">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>

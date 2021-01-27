---
title: 認証に関する問題点
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976854"
---
# <a name="authentication-issues"></a><span data-ttu-id="760e3-102">認証に関する問題点</span><span class="sxs-lookup"><span data-stu-id="760e3-102">Authentication issues</span></span>

<span data-ttu-id="760e3-103">**Azure Active Directory (Azure AD) セキュリティ トークン サービス (STS) から返される AADSTS エラー コードに関する情報をお探しですか?**</span><span class="sxs-lookup"><span data-stu-id="760e3-103">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="760e3-104">AADSTS エラーの説明、修正、およびいくつかの推奨される回避策については、「[Azure AD 認証および認証エラー コード](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="760e3-104">See [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>

<span data-ttu-id="760e3-105">認証エラーは、いくつかの異なる問題の結果である可能性があり、そのほとんどは 401 または 403 エラーを生成します。</span><span class="sxs-lookup"><span data-stu-id="760e3-105">Authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="760e3-106">たとえば、次の問題はすべて認証エラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="760e3-106">For example, the following issues can all lead to authorization errors:</span></span>

- <span data-ttu-id="760e3-107">間違った[アクセス トークンの取得フロー](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization)</span><span class="sxs-lookup"><span data-stu-id="760e3-107">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization)</span></span> 
- <span data-ttu-id="760e3-108">十分に構成されていない[アクセス許可スコープ](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)</span><span class="sxs-lookup"><span data-stu-id="760e3-108">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)</span></span> 
- <span data-ttu-id="760e3-109">[同意](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)がない</span><span class="sxs-lookup"><span data-stu-id="760e3-109">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="760e3-110">一般的な認証エラーを解決するには、発生しているエラーに最も近い以下の手順を試してください。</span><span class="sxs-lookup"><span data-stu-id="760e3-110">To resolve common authorization errors, try the steps provided below which most closely match the error you are receiving.</span></span> <span data-ttu-id="760e3-111">発生したエラーには、複数の手順が適用される場合があります。</span><span class="sxs-lookup"><span data-stu-id="760e3-111">More than one step may apply for an error you are receiving.</span></span>

<span data-ttu-id="760e3-112">**401 Unauthorized エラー: トークンは有効ですか?**</span><span class="sxs-lookup"><span data-stu-id="760e3-112">**401 Unauthorized error: Is your token valid?**</span></span>

<span data-ttu-id="760e3-113">アプリが要求の一部として、Microsoft Graph への有効なアクセス トークンを提示していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="760e3-113">Ensure that your app is presenting a valid access token to Microsoft Graph as part of the request.</span></span> <span data-ttu-id="760e3-114">このエラーは、多くの場合、HTTP 認証要求ヘッダーにアクセス トークンが存在しないか、トークンが無効であるか、有効期限が切れている可能性があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="760e3-114">This error often means that the access token may be missing in the HTTP authenticate request header or that the token is invalid or has expired.</span></span> <span data-ttu-id="760e3-115">アクセス トークンの取得には、Microsoft Authentication Library (MSAL) を使用することを強くお勧めします。</span><span class="sxs-lookup"><span data-stu-id="760e3-115">We strongly recommend that you use the Microsoft Authentication Library (MSAL) for access token acquisition.</span></span> <span data-ttu-id="760e3-116">さらに、このエラーは、個人の Microsoft アカウントに付与されている代理アクセス トークンを使用して、職場または学校のアカウント (組織のアカウント) のみをサポートする API にアクセスしようとする場合に発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="760e3-116">Additionally, this error may occur if you try to use a delegated access token granted to a personal Microsoft account to access an API that only supports work or school accounts (organizational accounts).</span></span>

<span data-ttu-id="760e3-117">**403 Forbidden エラー: 適切なアクセス許可のセットを選択しましたか?**</span><span class="sxs-lookup"><span data-stu-id="760e3-117">**403 Forbidden error: Have you chosen the right set of permissions?**</span></span>

<span data-ttu-id="760e3-118">アプリが呼び出す Microsoft Graph API に基づいて、適切なアクセス許可のセットを要求したことを確認します。</span><span class="sxs-lookup"><span data-stu-id="760e3-118">Ensure that you have requested the correct set of permissions based on the Microsoft Graph APIs your app calls.</span></span> <span data-ttu-id="760e3-119">推奨される最小特権アクセス許可は、Microsoft Graph API リファレンス メソッドのすべてのトピックで提供されます。</span><span class="sxs-lookup"><span data-stu-id="760e3-119">Recommended least-privileged permissions are provided in all the Microsoft Graph API reference method topics.</span></span> <span data-ttu-id="760e3-120">また、これらのアクセス許可は、ユーザーまたは管理者がアプリケーションに付与する必要があります。</span><span class="sxs-lookup"><span data-stu-id="760e3-120">Additionally, those permissions must be granted to the application by a user or an administrator.</span></span> <span data-ttu-id="760e3-121">通常、アクセス許可の付与は、同意ページまたは Azure Portal アプリケーションの登録ブレードの使用を通じて行われます。</span><span class="sxs-lookup"><span data-stu-id="760e3-121">Granting permissions normally happens through a consent page or usage of the Azure Portal application registration blade.</span></span> <span data-ttu-id="760e3-122">アプリケーションの **[設定]** ブレードで、**[必要なアクセス許可]** をクリックして、**[アクセス許可の付与]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="760e3-122">From the **Settings** blade for the application, click **Required Permissions**, and then click **Grant Permissions**.</span></span> <span data-ttu-id="760e3-123">詳しくは、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="760e3-123">For more information, see:</span></span>

- [<span data-ttu-id="760e3-124">Microsoft Graph のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="760e3-124">Microsoft Graph permissions</span></span>](https://docs.microsoft.com/graph/permissions-reference) 
- [<span data-ttu-id="760e3-125">Azure AD のアクセス許可と同意を理解する</span><span class="sxs-lookup"><span data-stu-id="760e3-125">Understanding Azure AD permissions and consent</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

<span data-ttu-id="760e3-126">**403 Forbidden エラー: アプリは選択されたアクセス許可と一致するトークンを取得しましたか?**</span><span class="sxs-lookup"><span data-stu-id="760e3-126">**403 Forbidden error: Did your app acquire a token to match chosen permissions?**</span></span>

<span data-ttu-id="760e3-127">要求されたアクセス許可の種類または与えられたアクセス許可の種類が、アプリが取得すアクセス トークンの種類と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="760e3-127">Ensure that the types of permissions requested or granted match the type of access token that your app acquires.</span></span> <span data-ttu-id="760e3-128">アプリのアクセス許可を要求して付与しますが、クライアント資格情報フロー トークンの代わりに、委任された対話型コード フロー トークンを使用する可能性があります。また、委任されたアクセス許可を要求して付与しますが、委任されたコード フロー トークンの代わりに、クライアント資格情報フロー トークンを使用する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="760e3-128">You might be requesting and granting app permissions but using delegated interactive code flow tokens instead of client credential flow tokens, or requesting and granting delegated permissions but using client credential flow tokens instead of delegated code flow tokens.</span></span>

<span data-ttu-id="760e3-129">トークンの取得に関する詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="760e3-129">For more information related to acquiring tokens, see:</span></span>

- [<span data-ttu-id="760e3-130">ユーザーに代わってアクセス権を取得し、アクセス許可を委任する</span><span class="sxs-lookup"><span data-stu-id="760e3-130">Get access on behalf of users and delegated permissions</span></span>](https://docs.microsoft.com/graph/auth-v2-user) 
- [<span data-ttu-id="760e3-131">Azure AD v2.0 - OAuth 2.0 承認コード フロー</span><span class="sxs-lookup"><span data-stu-id="760e3-131">Azure AD v2.0 - OAuth 2.0 authorization code flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [<span data-ttu-id="760e3-132">ユーザー (デーモン サービス) とアプリケーションのアクセス許可なしでアクセス権を取得する</span><span class="sxs-lookup"><span data-stu-id="760e3-132">Get access without a user (daemon service) and application permissions</span></span>](https://docs.microsoft.com/graph/auth-v2-service) 
- [<span data-ttu-id="760e3-133">Azure AD v2.0 - OAuth 2.0 クライアント資格情報フロー</span><span class="sxs-lookup"><span data-stu-id="760e3-133">Azure AD v2.0 - OAuth 2.0 client credentials flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

<span data-ttu-id="760e3-134">**403 Forbidden エラー: パスワードの再設定**</span><span class="sxs-lookup"><span data-stu-id="760e3-134">**403 Forbidden error: Resetting password**</span></span>

<span data-ttu-id="760e3-135">現在、ユーザー パスワードの再設定を許可するアプリケーションのアクセス許可デーモンサービス間のアクセス許可はありません。</span><span class="sxs-lookup"><span data-stu-id="760e3-135">Currently, there are no application permission daemon service-to-service permissions that allow resetting user passwords.</span></span> <span data-ttu-id="760e3-136">これらの API は、サインインしている管理者による対話型の委任されたコード フローを使用する場合にのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="760e3-136">These APIs are only supported using the interactive delegated code flows with a signed-in administrator.</span></span> <span data-ttu-id="760e3-137">詳細については、「[Microsoft Graph のアクセス許可](https://docs.microsoft.com/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="760e3-137">For more information, see [Microsoft Graph permissions](https://docs.microsoft.com/graph/permissions-reference).</span></span>

<span data-ttu-id="760e3-138">**403 Forbidden: ユーザーにアクセス権があり、ライセンスが付与されていますか?**</span><span class="sxs-lookup"><span data-stu-id="760e3-138">**403 Forbidden: Does the user have access and are they licensed?**</span></span>

<span data-ttu-id="760e3-139">委任されたコード フローの場合、Microsoft Graph は、アプリに付与されたアクセス許可とサインインしたユーザーが持つアクセス許可に基づいて、要求が許可されているかどうかを評価します。</span><span class="sxs-lookup"><span data-stu-id="760e3-139">For delegated code flows, Microsoft Graph evaluates whether the request has been allowed based on the permissions granted to the app and the permissions that the signed-in user has.</span></span> <span data-ttu-id="760e3-140">一般に、このエラーは、アクセスされているデータに対してユーザーにライセンスが付与されていない要求 **または** を実行するための十分な特権がユーザーにないことを示しています。</span><span class="sxs-lookup"><span data-stu-id="760e3-140">Generally, this error indicates that the user is not privileged enough to perform the request **or** the user is not licensed for the data being accessed.</span></span> <span data-ttu-id="760e3-141">必要なアクセス許可またはライセンスを持つユーザーのみが要求を正常に行うことができます。</span><span class="sxs-lookup"><span data-stu-id="760e3-141">Only users with the required permissions or licenses can make the request successfully.</span></span>

<span data-ttu-id="760e3-142">**403 Forbidden: 正しいリソース API を選択しましたか?**</span><span class="sxs-lookup"><span data-stu-id="760e3-142">**403 Forbidden: Did you select the correct resource API?**</span></span>

<span data-ttu-id="760e3-143">Microsoft Graph などの API サービスは、受信したアクセス トークンの *および* クレーム (オーディエンス) が、それ自体が予期する値と一致することを確認します。一致しない場合は、403 Forbidden エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="760e3-143">API services like Microsoft Graph check that the *aud* claim (audience) in the received access token matches the value it expects for itself, and if not, a 403 Forbidden error occurs.</span></span> <span data-ttu-id="760e3-144">このエラーの原因となる一般的な間違いは、Azure AD Graph API、Outlook API、または SharePoint/OneDrive API で取得したトークンを使用して Microsoft Graph を呼び出すことです (またはその逆)。</span><span class="sxs-lookup"><span data-stu-id="760e3-144">A common mistake resulting in this error is trying to use a token acquired for Azure AD Graph APIs, Outlook APIs, or SharePoint/OneDrive APIs to call Microsoft Graph (or vice versa).</span></span> <span data-ttu-id="760e3-145">アプリがトークンを取得しているリソース (またはスコープ) が、アプリが呼び出している API と一致していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="760e3-145">Ensure that the resource (or scope) your app is acquiring a token for matches the API that the app is calling.</span></span>

<span data-ttu-id="760e3-146">**400 要求が正しくありませんまたは 403 Forbidden: ユーザーは組織の条件付きアクセス (CA) ポリシーに準拠していますか?**</span><span class="sxs-lookup"><span data-stu-id="760e3-146">**400 Bad Request or 403 Forbidden: Does the user comply with their organization's conditional access (CA) policies?**</span></span>

<span data-ttu-id="760e3-147">組織の条件付きアクセス (CA) ポリシーに基づいて、アプリを使用して Microsoft Graph リソースにアクセスするユーザーは、アプリが最初に取得したアクセス トークンに存在しない追加情報を要求される場合があります。</span><span class="sxs-lookup"><span data-stu-id="760e3-147">Based on an organization's conditional access (CA) policies, a user accessing Microsoft Graph resources via your app may be challenged for additional information that is not present in the access token your app originally acquired.</span></span> <span data-ttu-id="760e3-148">この場合、アプリはアクセス トークンの取得中に **400 と *interaction_required*** エラーを受け取り、Microsoft Graph を呼び出すときに **403 と *insufficient_claims*** エラーを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="760e3-148">In this case, your app receives a **400 with an *interaction_required*** error during access token acquisition or a **403 with *insufficient_claims*** error when calling Microsoft Graph.</span></span> <span data-ttu-id="760e3-149">どちらの場合も、エラー応答には、認証エンドポイントに提示して、ユーザーに追加情報 (多要素認証やデバイス登録など) を要求できる追加情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="760e3-149">In both cases, the error response contains additional information that can be presented to the authorized endpoint to challenge the user for additional information (like multi-factor authentication or device enrollment).</span></span>

<span data-ttu-id="760e3-150">条件付きアクセスに関する詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="760e3-150">For more information related to conditional access, see:</span></span>

- [<span data-ttu-id="760e3-151">MSAL を使用して、条件付きアクセスの課題を処理する</span><span class="sxs-lookup"><span data-stu-id="760e3-151">Handling conditional access challenges using MSAL</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [<span data-ttu-id="760e3-152">Azure Active Directory 条件付きアクセスの開発者ガイダンス</span><span class="sxs-lookup"><span data-stu-id="760e3-152">Developer guidance for Azure Active Directory conditional access</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

<span data-ttu-id="760e3-153">\**_Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) のサポートの終了_* _</span><span class="sxs-lookup"><span data-stu-id="760e3-153">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

- <span data-ttu-id="760e3-154">2020 年 6 月 30 日以降、Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) に新しい機能を追加しなくなります。</span><span class="sxs-lookup"><span data-stu-id="760e3-154">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="760e3-155">テクニカル サポートおよびセキュリティ更新プログラムは引き続き提供されますが、機能の更新プログラムは提供されなくなります。</span><span class="sxs-lookup"><span data-stu-id="760e3-155">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="760e3-156">2022 年 6月 30 日に ADAL および AAD Graph のサポートは終了し、以降はテクニカル サポートやセキュリティ更新プログラムは提供されなくなります。</span><span class="sxs-lookup"><span data-stu-id="760e3-156">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span>
    - <span data-ttu-id="760e3-157">既存の OS バージョンで ADAL を使用するアプリは、この期間以降も引き続き機能しますが、テクニカル サポートやセキュリティ更新プログラムは提供されません。</span><span class="sxs-lookup"><span data-stu-id="760e3-157">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>
    - <span data-ttu-id="760e3-158">これ以降に AAD Graph を使用するアプリは、AAD Graph エンドポイントからの応答を受信しなくなる場合があります。</span><span class="sxs-lookup"><span data-stu-id="760e3-158">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint.</span></span>

<span data-ttu-id="760e3-159">_ *ADAL 移行*\*</span><span class="sxs-lookup"><span data-stu-id="760e3-159">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="760e3-160">最新の機能とセキュリティ更新プログラムを備えた[Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) に更新することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="760e3-160">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span> <span data-ttu-id="760e3-161">この推奨事項は、Microsoft がサポート終了期限までにアプリケーションを MSAL に移行することに関連しています。</span><span class="sxs-lookup"><span data-stu-id="760e3-161">This recommendation is in the context of Microsoft migrating its applications to MSAL by the end-of-support deadline.</span></span> <span data-ttu-id="760e3-162">Microsoft アプリを MSAL に移行する目的は、アプリが継続的に MSAL の強化されたセキュリティと機能を利用できることを保証するためです。</span><span class="sxs-lookup"><span data-stu-id="760e3-162">The objective of Microsoft apps' migration to MSAL is to ensure that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

- [<span data-ttu-id="760e3-163">ADAL の FAQ を読む</span><span class="sxs-lookup"><span data-stu-id="760e3-163">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [<span data-ttu-id="760e3-164">プラットフォームごとにアプリを移行する方法に関する詳細情報</span><span class="sxs-lookup"><span data-stu-id="760e3-164">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- <span data-ttu-id="760e3-165">どのアプリが ADAL を使用しているかを理解するためにサポートが必要な場合は、すべてのアプリのソース コードを確認し、該当する場合は、独立系ソフトウェア ベンダー (ISV) またはアプリ プロバイダーに連絡することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="760e3-165">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="760e3-166">Microsoft サポートでは、テナントにあるすべての Microsoft ADAL 以外のアプリのリストも提供できます。</span><span class="sxs-lookup"><span data-stu-id="760e3-166">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="760e3-167">**AAD Graph の移行**</span><span class="sxs-lookup"><span data-stu-id="760e3-167">**AAD Graph Migration**</span></span>

<span data-ttu-id="760e3-168">AAD Graph を使用しているアプリケーションの場合は、ガイダンスに従って [Azure AD Graph アプリを Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true) に移行してください。</span><span class="sxs-lookup"><span data-stu-id="760e3-168">For applications that are using AAD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).</span></span>

- <span data-ttu-id="760e3-169">[移行のチェックリストは、開始ポイントを提供します](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。</span><span class="sxs-lookup"><span data-stu-id="760e3-169">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
- <span data-ttu-id="760e3-170">Azure アプリの登録ポータルには、AAD Graph を使用しているアプリケーションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="760e3-170">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="760e3-171">アプリのすべてのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="760e3-171">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="760e3-172">Microsoft のサポートでは、テナントでのすべての AAD Graph の使用状況に関する情報を提供することもできます。</span><span class="sxs-lookup"><span data-stu-id="760e3-172">Microsoft support can also provide you the information of all AAD Graph usage in your tenant.</span></span>

 











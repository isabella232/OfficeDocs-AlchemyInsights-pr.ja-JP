---
title: 認証ライブラリの操作
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038238"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="7247d-102">認証ライブラリの操作</span><span class="sxs-lookup"><span data-stu-id="7247d-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="7247d-103">Microsoft 認証ライブラリ (MSAL) の問題を解決するには、次の推奨手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="7247d-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="7247d-104">**MSAL の操作**: [Microsoft ID プラットフォーム認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - この記事では、複数のアプリケーションの種類に対する Microsoft 認証ライブラリのサポートについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7247d-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="7247d-105">これには、ライブラリのソース コードへのリンク、アプリのプロジェクトのパッケージを取得する場所を含み、ライブラリがユーザーのサインイン(認証)か、保護された Web API へのアクセス (承認)をサポートするのかどうか、あるいはその両方がサポートされているのかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="7247d-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="7247d-106">**トラブルシューティング認証**: MSAL は、さまざまなアプリケーション シナリオで使用する複数の認証フローをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="7247d-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="7247d-107">クライアント アプリケーションの構築方法によっては、MSAL は Microsoft ID プラットフォームでサポートされる 1 つ以上の認証フローを使用できます。</span><span class="sxs-lookup"><span data-stu-id="7247d-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="7247d-108">これらのフローは、いくつかの種類のトークンおよび承認コードを生成する可能性があり、それらを動作させるためには、異なるトークンが必要です。</span><span class="sxs-lookup"><span data-stu-id="7247d-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="7247d-109">**アクセス トークン**: 「[Microsoft ID プラットフォームのアクセス トークン](https://docs.microsoft.com/azure/active-directory/develop/access-tokens)」 - API がアクセス トークン内のクレームを検証および使用する方法を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7247d-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="7247d-110">特に明示されている場合を除き、この記事のすべてのドキュメントは、登録した API に対して発行されるトークンにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="7247d-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="7247d-111">これは、Microsoft 所有の API で発行されるトークンには適用されません。また、これらのトークンを使用して、作成した API に対して Microsoft ID プラットフォームがトークンを発行する方法を検証することもできません。</span><span class="sxs-lookup"><span data-stu-id="7247d-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="7247d-112">**Azure Active Directory 認証ライブラリ (ADAL) のサポートが終了しました**</span><span class="sxs-lookup"><span data-stu-id="7247d-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="7247d-113">**2020 年 6 月 30 日以降、** ADAL および Azure AD Graph に新しい機能は追加されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7247d-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="7247d-114">テクニカル サポートおよびセキュリティ更新プログラムは引き続き提供されますが、機能の更新プログラムは提供されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7247d-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="7247d-115">**2022 年 6月 30 日以降、** ADAL および Azure AD Graph のサポートは終了し、テクニカル サポートやセキュリティ更新プログラムは提供されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7247d-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="7247d-116">既存の OS バージョンで ADAL を使用するアプリは、この期間以降も引き続き機能しますが、*テクニカル サポートやセキュリティ更新プログラムの提供* は行われません。</span><span class="sxs-lookup"><span data-stu-id="7247d-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="7247d-117">これ以降に Azure AD Graph を使用するアプリは、Azure AD Graph エンドポイントからの応答を受信しなくなる場合があります。</span><span class="sxs-lookup"><span data-stu-id="7247d-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="7247d-118">**ADAL 移行**</span><span class="sxs-lookup"><span data-stu-id="7247d-118">**ADAL Migration**</span></span>

- <span data-ttu-id="7247d-119">最新の機能とセキュリティ更新プログラムを備えた MSAL に更新することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="7247d-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="7247d-120">Microsoft アプリを使用している場合は、Microsoft がサポート終了期限までにアプリを MSAL に移行していることを確認し、継続的に MSAL の強化されたセキュリティと機能を利用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="7247d-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="7247d-121">[ADAL の FAQ を確認します](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。</span><span class="sxs-lookup"><span data-stu-id="7247d-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="7247d-122">[プラットフォームごとにアプリを移行する方法について説明します](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)。</span><span class="sxs-lookup"><span data-stu-id="7247d-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="7247d-123">アプリのプラットフォームのガイドを読んだ後、他にも質問がある場合は、[azure-ad-adal-deprecation] タグを使って、「[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html)」 に投稿するか、ライブラリの GitHub リポジトリで問題を開くことができます。</span><span class="sxs-lookup"><span data-stu-id="7247d-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="7247d-124">各ライブラリのリポジトリへのリンクについては、**MSAL の概要** 記事の、「[言語とフレームワーク](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks)」セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="7247d-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="7247d-125">**どのアプリが ADAL を使用しているかを理解するためにサポートが必要な場合は**、すべてのアプリのソース コードを確認することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="7247d-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="7247d-126">該当する場合は、独立系ソフトウェア ベンダー (ISV) またはアプリ プロバイダーに問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="7247d-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="7247d-127">Microsoft サポートでは、テナントにあるすべての Microsoft ADAL 以外のアプリのリストも提供できます。</span><span class="sxs-lookup"><span data-stu-id="7247d-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>








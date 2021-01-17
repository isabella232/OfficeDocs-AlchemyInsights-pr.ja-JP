---
title: 自分のオンプレミス アプリとシームレスな SSO の統合に関する問題
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868790"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="2fd2c-102">自分のオンプレミス アプリとシームレスな SSO の統合に関する問題</span><span class="sxs-lookup"><span data-stu-id="2fd2c-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="2fd2c-103">オンプレミス アプリケーションとのシームレスな SSO の統合に関する問題をトラブルシューティングするには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="2fd2c-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="2fd2c-104">**推奨される手順**</span><span class="sxs-lookup"><span data-stu-id="2fd2c-104">**Recommended steps**</span></span>

1. <span data-ttu-id="2fd2c-105">**アプリケーション プロキシを使用したシングル サインオン** 用に **オンプレミス アプリケーション** を構成するには、「[Password vaulting for single sign-on with Application Proxy (アプリケーション プロキシを使用したシングル サインオン用のパスワード管理)](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fd2c-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="2fd2c-106">**アプリケーション プロキシの問題のトラブルシューティング**: アプリケーション プロキシ コネクタが正しく設定されているかどうかを判断するために、トラブルシューティング フロー「[Debug Application Proxy Connector issues (アプリケーション プロキシ コネクタの問題のデバッグ)](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)」の確認から始めることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="2fd2c-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="2fd2c-107">依然としてアプリケーションへの接続に問題がある場合は、「[Debug Application Proxy application issues (アプリケーション プロキシ アプリケーションの問題のデバッグ)](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)」に記載されているトラブルシューティング手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="2fd2c-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="2fd2c-108">以下のブラウザ デバッグ ツールを使用し、[CORS の問題を特定](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues)できます。</span><span class="sxs-lookup"><span data-stu-id="2fd2c-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="2fd2c-109">ブラウザーを起動し、Web アプリを閲覧します。</span><span class="sxs-lookup"><span data-stu-id="2fd2c-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="2fd2c-110">**F12 キー** を押して、デバッグ コンソールを起動します。</span><span class="sxs-lookup"><span data-stu-id="2fd2c-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="2fd2c-111">トランザクションを再現し、コンソールのメッセージを確認します。</span><span class="sxs-lookup"><span data-stu-id="2fd2c-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="2fd2c-112">CORS の違反により、オリジンに関するコンソール エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="2fd2c-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="2fd2c-113">CORS の問題の一部は、アプリが認証のために login.microsoftonline.com にリダイレクトされたり、アクセス トークンが期限切れになったりする場合など、解決できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="2fd2c-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="2fd2c-114">その後、CORS の呼び出しは失敗します。</span><span class="sxs-lookup"><span data-stu-id="2fd2c-114">The CORS call then fails.</span></span> <span data-ttu-id="2fd2c-115">ユーザーのセッション中にアクセス トークンの有効期限が切れないようにアクセス トークンの有効期限を延長することが、このシナリオの回避策です。</span><span class="sxs-lookup"><span data-stu-id="2fd2c-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="2fd2c-116">これを行う方法の詳細については、「[Configurable token lifetimes in Microsoft identity platform (Microsoft ID プラットフォームで構成可能なトークンの有効期限)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fd2c-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="2fd2c-117">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="2fd2c-117">**Recommended documents**</span></span>

- [<span data-ttu-id="2fd2c-118"> アプリケーション プロキシ アプリケーションへのシングル サインオンの構成方法</span><span class="sxs-lookup"><span data-stu-id="2fd2c-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="2fd2c-119">アプリケーション プロキシを使用したオンプレミス アプリケーションの SAML シングル サインオン</span><span class="sxs-lookup"><span data-stu-id="2fd2c-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="2fd2c-120">Azure Active Directory アプリケーション プロキシの CORS の問題を理解し、解決する</span><span class="sxs-lookup"><span data-stu-id="2fd2c-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="2fd2c-121">アプリケーション プロキシの Kerberos の制約付き委任構成のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="2fd2c-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
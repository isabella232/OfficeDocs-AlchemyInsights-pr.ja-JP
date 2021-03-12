---
title: パスワードベースのシームレス シングル サインオン (SSO) の問題のトラブルシューティング
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714920"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="e0759-102">パスワードベースのシームレス シングル サインオン (SSO) の問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="e0759-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="e0759-103">パスワードベースの SSO の基礎の詳細については、「[Azure Active Directory SSO を使用したパスワードベースの 認証](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0759-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="e0759-104">**パスワードベースの SSO を構成する**</span><span class="sxs-lookup"><span data-stu-id="e0759-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="e0759-105">[パスワードベースのシングル サインオン ドメイン](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - この記事では、パスワードベースの SSO オプションについて詳しく説明します。</span><span class="sxs-lookup"><span data-stu-id="e0759-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="e0759-106">追加するアプリケーションでカスタム構成が必要であり、パスワードベースの SSO を使用する必要がある場合は、この記事をお読みください。</span><span class="sxs-lookup"><span data-stu-id="e0759-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="e0759-107">[オンプレミス アプリ用にパスワード ベースのシングル サインオンを構成する](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - アプリケーション プロキシは、いくつかのシングル サインオン モードをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="e0759-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="e0759-108">パスワードベースのサインオンは、認証にユーザー名/パスワードの組み合わせを使用するアプリケーションを対象とします。</span><span class="sxs-lookup"><span data-stu-id="e0759-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="e0759-109">アプリケーションにパスワードベースのサインオンを構成する場合、ユーザーはオンプレミス アプリケーションに一度サインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0759-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="e0759-110">その後、Azure Active Directory はサインイン情報を保存し、ユーザーがリモートでアクセスするときに、その情報を自動的にアプリケーションに提供します。</span><span class="sxs-lookup"><span data-stu-id="e0759-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="e0759-111">アプリケーション プロキシを使用して、アプリを既に公開しテストしている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0759-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="e0759-112">そうでない場合は、「[Azure AD アプリケーション プロキシを使用してアプリケーションを公開する](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)」の手順に従い、オンプレミス アプリ用のパスワード ベース SSO の構成を続行します。</span><span class="sxs-lookup"><span data-stu-id="e0759-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="e0759-113">パスワードベース SSO のトラブルシューティングを行う方法については、「[Azure AD において、パスワードベースのシングル サインオンのトラブルシューティングを行う](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0759-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>

---
title: シームレス SSO のユーザー サインインに関する問題
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935228"
---
# <a name="seamless-sso-user-sign-in-issues"></a><span data-ttu-id="247d0-102">シームレス SSO のユーザー サインインに関する問題</span><span class="sxs-lookup"><span data-stu-id="247d0-102">Seamless SSO user sign-in issues</span></span>

<span data-ttu-id="247d0-103">ユーザーが認証されると、ブラウザーはユーザーの認証情報をキャッシュし、アプリケーションが同じブラウザーで同じアカウントを使用して自動的にサインインするようにします。</span><span class="sxs-lookup"><span data-stu-id="247d0-103">After the user is authenticated, the browser will cache the user's credentials, so that on the same browser, the application will automatically sign-in with the same account.</span></span> <span data-ttu-id="247d0-104">これにより、別のユーザーまたは単一のユーザーが 1 つのデバイスで複数のアカウントにログインするのが難しいことがあります。</span><span class="sxs-lookup"><span data-stu-id="247d0-104">This may make it difficult for another user or a single user to log into multiple accounts on one device.</span></span> <span data-ttu-id="247d0-105">この問題を解決するには、次の手順を実行します。1.</span><span class="sxs-lookup"><span data-stu-id="247d0-105">To solve this: 1.</span></span> <span data-ttu-id="247d0-106">別のブラウザーでサインインします。</span><span class="sxs-lookup"><span data-stu-id="247d0-106">Try signing in on another browser.</span></span> <span data-ttu-id="247d0-107">2.</span><span class="sxs-lookup"><span data-stu-id="247d0-107">2.</span></span> <span data-ttu-id="247d0-108">ブラウザーのキャッシュとクッキーを消去し、もう一度サインインします。</span><span class="sxs-lookup"><span data-stu-id="247d0-108">Clear the browser's cache and/or cookies and try signing in again.</span></span>

<span data-ttu-id="247d0-109">サインインに関する問題が引き続き発生する場合、診断と解決手順を自動化するために次のことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="247d0-109">If you are still experiencing sign-in issues, we recommend the following to diagnose and automate the resolution steps:</span></span>

1. <span data-ttu-id="247d0-110">[My Apps Secure Browser Extension](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) をインストールします。これをインストールすると、Azure portal でテスト体験を使用するとき、Azure Active Directory (Azure AD) からより良い診断と解決策が得られます。</span><span class="sxs-lookup"><span data-stu-id="247d0-110">Install the [My Apps Secure Browser Extension](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) to help Azure Active Directory (Azure AD) to provide better diagnosis and resolutions when using the testing experience in the Azure portal.</span></span>
2. <span data-ttu-id="247d0-111">Azure portal のアプリ構成ページにあるテスト体験を使用し、エラーを再現します。</span><span class="sxs-lookup"><span data-stu-id="247d0-111">Reproduce the error using the testing experience in the app configuration page in the Azure portal.</span></span> <span data-ttu-id="247d0-112">詳細については、[SAML ベースのシングル サインオン アプリケーションをデバッグする](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)方法に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="247d0-112">To learn more, see [Debug SAML-based single sign-on applications](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).</span></span>
3. <span data-ttu-id="247d0-113">My Apps Secure Browser Extension を使用して、Azure portal でテスト体験を使用する場合は、**手順 4 を省略** できます。</span><span class="sxs-lookup"><span data-stu-id="247d0-113">If you use the testing experience in the Azure portal with the My Apps Secure Browser Extension, you can **skip step 4**.</span></span>
4. <span data-ttu-id="247d0-114">[SAML ベースのシングル サインオンの構成] ページを開くには、次の手順を行います。</span><span class="sxs-lookup"><span data-stu-id="247d0-114">To open the SAML-based single sign-on configuration page:</span></span>
    - <span data-ttu-id="247d0-115">[Azure portal](https://portal.azure.com/) を開き、**グローバル管理者**、または **共同管理者** としてサインインします。</span><span class="sxs-lookup"><span data-stu-id="247d0-115">Open the [Azure portal](https://portal.azure.com/) and sign in as a **Global Administrator** or **Coadmin**.</span></span>
    - <span data-ttu-id="247d0-116">左側のメイン ナビゲーション メニューの上部にある **[すべてのサービス]** を選択して **[Azure Active Directory 拡張機能]** を開きます。</span><span class="sxs-lookup"><span data-stu-id="247d0-116">Open the **Azure Active Directory Extension** by selecting **All services** at the top of the main left-side navigation menu.</span></span>
    - <span data-ttu-id="247d0-117">フィルター検索ボックスに "Azure Active Directory" と入力し、**[Azure Active Directory]** 項目を選択します。</span><span class="sxs-lookup"><span data-stu-id="247d0-117">Type "Azure Active Directory" in the filter search box and select the **Azure Active Directory** item.</span></span>
    - <span data-ttu-id="247d0-118">Azure Active Directory の左側のナビゲーション メニューから **[エンタープライズ アプリケーション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="247d0-118">Select **Enterprise Applications** from the Azure Active Directory left-hand navigation menu.</span></span>
    - <span data-ttu-id="247d0-119">**[すべてのアプリケーション]** を選択して、すべてのアプリケーションの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="247d0-119">Select **All Applications** to view a list of all your applications.</span></span> <span data-ttu-id="247d0-120">ここに表示したいアプリケーションが表示されない場合は、**[All Applications List (すべてのアプリケーション リスト)]** の上部にある **[フィルター]** コントロールを使用して、**[表示]** オプションを **[すべてのアプリケーション]** に設定します。</span><span class="sxs-lookup"><span data-stu-id="247d0-120">If you do not see the application you want show up here, use the **Filter** control at the top of the **All Applications List** and set the **Show** option to **All Applications**.</span></span>
    - <span data-ttu-id="247d0-121">シングル サインオンを構成するアプリケーションを選択します。</span><span class="sxs-lookup"><span data-stu-id="247d0-121">Select the application you want to configure for single sign-on.</span></span>
    - <span data-ttu-id="247d0-122">アプリケーションが読み込まれた後、アプリケーションの左側にあるナビゲーション メニューで **[シングル サインオン]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="247d0-122">After the application loads, select **Single sign-on** from the application’s left-hand navigation menu.</span></span>
    - <span data-ttu-id="247d0-123">**[SAML ベースの SSO]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="247d0-123">Select **SAML-based SSO**.</span></span>
5. <span data-ttu-id="247d0-124">エラーに基づいて推奨される次の手順の詳細については、「[SAML ベースのシングル サインオンで構成されたアプリへのサインインに関する問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="247d0-124">Based on the error, to learn more about the recommended steps to follow, see [Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).</span></span>
6. <span data-ttu-id="247d0-125">その他のユーザー サインに関する問題のトラブルシューティングを行うには、次のガイダンスを参照してください。</span><span class="sxs-lookup"><span data-stu-id="247d0-125">To troubleshoot other user sign-issues refer to the following guidance:</span></span>
    - [<span data-ttu-id="247d0-126">シングル サインオンの SAML プロトコル</span><span class="sxs-lookup"><span data-stu-id="247d0-126">Single Sign-On SAML protocol</span></span>](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [<span data-ttu-id="247d0-127">方法: Azure Active Directory レポートを使用してサインイン エラーをトラブルシューティングする</span><span class="sxs-lookup"><span data-stu-id="247d0-127">How to: Troubleshoot sign-in errors using Azure Active Directory reports</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [<span data-ttu-id="247d0-128">予期しない同意プロンプト</span><span class="sxs-lookup"><span data-stu-id="247d0-128">Unexpected consent prompt</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [<span data-ttu-id="247d0-129">ユーザーの同意エラー</span><span class="sxs-lookup"><span data-stu-id="247d0-129">User consent error</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [<span data-ttu-id="247d0-130">マイ アプリからのサインインに関する問題</span><span class="sxs-lookup"><span data-stu-id="247d0-130">Problems signing in from My Apps</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [<span data-ttu-id="247d0-131">アプリケーションのサインイン ページでのエラー</span><span class="sxs-lookup"><span data-stu-id="247d0-131">Error on application sign-in page</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [<span data-ttu-id="247d0-132">Microsoft アプリへのサインインに関する問題</span><span class="sxs-lookup"><span data-stu-id="247d0-132">Problem signing into a Microsoft App</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)

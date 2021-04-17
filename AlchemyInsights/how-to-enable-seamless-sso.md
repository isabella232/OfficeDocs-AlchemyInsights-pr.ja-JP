---
title: シームレスな SSO を有効にする方法
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 565ec53a3d9f8863562ac828e21a4a153c61ae88
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825736"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="e14be-102">シームレスな SSO を有効にする方法</span><span class="sxs-lookup"><span data-stu-id="e14be-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="e14be-103">シームレスな SSO は、[Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) を使用して有効にします。</span><span class="sxs-lookup"><span data-stu-id="e14be-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="e14be-p101">Azure AD Connect を新規でインストールする場合、[カスタム インストール パス](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)を選択します。**[ユーザー サインイン]** ページで、**[シングル サインオンを有効にする]** オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="e14be-p101">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom). At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="e14be-106">シームレスな SSO が正しく有効化されたかを確認するには:</span><span class="sxs-lookup"><span data-stu-id="e14be-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="e14be-107">[Azure Active Directory 管理センター](https://aad.portal.azure.com)に全体管理者としてサインインします。</span><span class="sxs-lookup"><span data-stu-id="e14be-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="e14be-108">左のウィンドウの **[Azure Active Directory]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e14be-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="e14be-109">シームレスなシングル サインオンが **[有効]** になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="e14be-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="e14be-110">詳細については、[Azure Active Directory シームレス シングル サインオン: クイック スタート](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e14be-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  
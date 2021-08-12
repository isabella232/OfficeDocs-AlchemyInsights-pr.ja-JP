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
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972829"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>パスワードベースのシームレス シングル サインオン (SSO) の問題のトラブルシューティング

パスワードベースの SSO の基礎の詳細については、「[Azure Active Directory SSO を使用したパスワードベースの 認証](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)」を参照してください。

**パスワードベースの SSO を構成する**

1. [パスワードベースのシングル サインオン ドメイン](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - この記事では、パスワードベースの SSO オプションについて詳しく説明します。 追加するアプリケーションでカスタム構成が必要であり、パスワードベースの SSO を使用する必要がある場合は、この記事をお読みください。
2. [オンプレミス アプリ用にパスワード ベースのシングル サインオンを構成する](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - アプリケーション プロキシは、いくつかのシングル サインオン モードをサポートしています。 パスワードベースのサインオンは、認証にユーザー名/パスワードの組み合わせを使用するアプリケーションを対象とします。 アプリケーションにパスワードベースのサインオンを構成する場合、ユーザーはオンプレミス アプリケーションに一度サインインする必要があります。 その後、Azure Active Directory はサインイン情報を保存し、ユーザーがリモートでアクセスするときに、その情報を自動的にアプリケーションに提供します。
    - アプリケーション プロキシを使用して、アプリを既に公開しテストしている必要があります。 そうでない場合は、「[Azure AD アプリケーション プロキシを使用してアプリケーションを公開する](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)」の手順に従い、オンプレミス アプリ用のパスワード ベース SSO の構成を続行します。

パスワードベース SSO のトラブルシューティングを行う方法については、「[Azure AD において、パスワードベースのシングル サインオンのトラブルシューティングを行う](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)」を参照してください。

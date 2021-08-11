---
title: アプリ プロキシの構成
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
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951570"
---
# <a name="app-proxy-configuration"></a>アプリ プロキシの構成

1. オンプレミス アプリケーションをクラウドに公開するように Azure AD 内でアプリケーション プロキシ アプリケーションを設定する方法については、「[アプリケーション プロキシ アプリケーションの構成方法](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)」を参照してください。
2. シングル サインオン (SSO) を使用すると、ユーザーは複数回認証しなくてもアプリケーションにアクセスできます。 これにより、Azure Active Directory に対してクラウド上で単一の認証を行うことができ、サービスまたはコネクタがユーザーになりすますことで、アプリケーションからの追加の認証確認を完了できます。 詳細については、「[アプリケーション プロキシ アプリケーションへのシングル サインオンの構成方法](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)」を参照してください。
3. [この記事](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem)を使用して、新しいアプリケーション プロキシ アプリケーションの作成時に発生する一般的な問題のトラブルシューティングを行ってください。
4. アプリケーションに対するバックエンド認証のセットアップで問題が発生した場合は、[アプリケーション プロキシの Kerberos 制約付き委任構成のトラブルシューティングを行う](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to)か、「[PingAccess を使用してアプリケーションを構成する](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to)」のガイダンスに従って問題を解決する必要があります。

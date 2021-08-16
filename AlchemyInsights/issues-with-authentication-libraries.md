---
title: 認証ライブラリに関する問題
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028009"
---
# <a name="issues-with-authentication-libraries"></a>認証ライブラリに関する問題

1. [Microsoft ID プラットフォーム認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)には、Microsoft がサポートする互換性のあるクライアントおよびミドルウェア ライブラリが一覧表示されます。
2. Microsoft Authentication Library (MSAL) は、さまざまなアプリケーション シナリオで使用する複数の[認証フロー](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows)をサポートしています。
3. トークンを認証して取得するには、コードで新しいパブリックまたは機密のクライアント アプリケーションを初期化します。 Microsoft Authentication Library (MSAL) でクライアント アプリを初期化するときに、いくつかの構成オプションを設定できます。 詳細については、「[アプリケーション構成オプション](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)」を参照してください。

**Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) のサポートの終了** _

**2020 年 6 月 30 日以降**、ADAL および Azure AD Graph に新しい機能は追加されなくなります。 テクニカル サポートおよびセキュリティ更新プログラムは引き続き提供されますが、機能の更新プログラムは提供されなくなります。

**2022 年 6月 30 日以降**、ADAL と Azure AD Graph のサポートは終了し、テクニカル サポートやセキュリティ更新プログラムは提供されなくなります。

既存の OS バージョンで ADAL を使用するアプリは、この期間以降も引き続き機能しますが、*テクニカル サポートやセキュリティ更新プログラムの提供* は行われません。

これ以降に Azure AD Graph を使用するアプリは、Azure AD Graph エンドポイントからの応答を受信しなくなる場合があります。

**ADAL 移行**

最新の機能とセキュリティ更新プログラムを備えた[Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) に更新することをお勧めします。

Microsoft アプリを使用している場合は、Microsoft がサポート終了期限までにアプリケーションを MSAL に移行していることを確認し、継続的に MSAL の強化されたセキュリティと機能を利用できるようにします。

詳しくは、以下を参照してください。

1. [ADAL の FAQ を読む](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [プラットフォームごとにアプリを移行する方法に関する詳細情報](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. どのアプリが ADAL を使用しているかを理解するためにサポートが必要な場合は、すべてのアプリのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。 Microsoft サポートでは、テナントにあるすべての Microsoft ADAL 以外のアプリのリストも提供できます。

**AAD Graph の移行**

Azure AD Graph を使用しているアプリケーションの場合は、ガイダンスに従って [Azure AD Graph アプリを Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview) に移行してください。

1. [移行のチェックリストは、開始ポイントを提供します](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。
2. Azure アプリの登録ポータルには、AAD Graph を使用しているアプリケーションが表示されます。 アプリのすべてのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。 Microsoft のサポートでは、テナントでのすべての AAD Graph の使用状況のリストを提供することもできます。
3. アプリから Microsoft Graph のデータにアクセスする場合、ユーザーまたは管理者は、同意のプロセスを通してそのアプリに正しいアクセス許可を付与する必要があります。 [Microsoft Graph のアクセス許可リファレンス](https://docs.microsoft.com/graph/permissions-reference)では、Microsoft Graph API の各主要なセットに関連付けられているアクセス許可について説明します。 また、アクセス許可の使用方法に関するガイダンスを提供しています。

---
title: Microsoft Graph API に関する問題
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/29/2021
ms.locfileid: "50053090"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graph API に関する問題

このトピックは、Azure AD Graph API をまだ使用している開発者にも当てはまります。 ただし、すべてのディレクトリ、ID、およびアクセス管理シナリオで Microsoft Graph を使用することを **強く** お勧めします。

**認証または許可に関する問題**

- アプリが Microsoft Graph を呼び出すための **トークンを取得できない** 場合、**アクセス トークンの取得に関する問題 (認証)** Microsoft Graph カテゴリを選択して、このトピックに関するより具体的なヘルプとサポートを受けることができます。
- Microsoft Graph を呼び出しているときにアプリが **401 または 403 の認証エラー** を受信している場合は、**アクセス拒否エラー (認証)** Microsoft Graph API カテゴリを選択すると、このトピックに関するより具体的なヘルプとサポートを受けることができます。

**Microsoft Graph を使用したいが、開始点がわかりません**

- [Microsoft Graph の概要](https://docs.microsoft.com/graph/overview)
- [Microsoft Graph の ID およびアクセス管理の概要](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph アプリの作成の開始](https://docs.microsoft.com/graph/)
- **Microsoft Graph エクスプローラー** - テナントまたはデモ テナントで Microsoft Graph API をテストする

**Microsoft Graph を使用したいが、必要な v1.0 ディレクトリ API をサポートしていますか?**

Microsoft Graph は、ディレクトリ、ID、およびアクセス管理に推奨される API です。 しかし、Azure AD Graph と Microsoft Graph にはまだいくつかのギャップがあります。 次の記事を確認してください。これらの記事では、選択に役立つ最新の違いを強調しています。

- [Azure AD Graph と Microsoft Graph のリソースの種類の違い](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graph と Microsoft Graph のプロパティの違い](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD と Microsoft Graph のメソッドの違い](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**呼び出している API が機能しません。詳細なテストはどこで実行できますか?**

**Microsoft Graph エクスプローラー** - テナントまたはデモ テナントで Microsoft Graph API をテストし、Microsoft Graph エクスプローラーで **サンプル クエリ** を確認します。

**アプリは遅すぎて、制限されています。改善する方法はありますか?**

シナリオに応じて、アプリケーションのパフォーマンスを向上させ、場合によっては、サービスによって制限される可能性を低くする (呼び出しが多すぎる場合) ために、各種のオプションを自由に使用できます。

- [Microsoft Graph のベスト プラクティス](https://docs.microsoft.com/graph/best-practices-concept)
- [バッチ要求](https://docs.microsoft.com/graph/json-batching)
- [デルタ クエリによる変更の追跡](https://docs.microsoft.com/graph/delta-query-overview)
- [Web フックによる変更の通知を受ける](https://docs.microsoft.com/graph/webhooks)
- [調整ガイダンス](https://docs.microsoft.com/graph/throttling)

**エラーおよび既知の問題に関する詳細情報はどこで確認できますか?**

- [Microsoft Graph のエラー応答情報](https://docs.microsoft.com/graph/errors)
- [Microsoft Graph に関する既知の問題](https://docs.microsoft.com/graph/known-issues)

**サービスの可用性と接続状態はどこで確認できますか?**

Microsoft Graph を介してアクセスできる基礎となるサービスのサービス可用性と接続性は、Microsoft Graph の全体的な可用性とパフォーマンスに影響を与える可能性があります。

- Azure Active Directory サービスの正常性については、「[Azure 状態ページ](https://azure.microsoft.com/status/)にリストされている **セキュリティ + ID** サービスの状態を確認します。
- Microsoft Graph に貢献する Office サービスについては、「[Office サービス正常性ダッシュボード](https://portal.office.com/adminportal/home#/servicehealth)にリストされているサービスの状態を確認します。

Microsoft Graph の認証エラーは、いくつかの異なる問題の結果である可能性があり、そのほとんどは 401または 403 エラーを生成します。 たとえば、次の場合はすべて承認エラーが発生する可能性があります。

- 間違った[アクセス トークンの取得フロー](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- 十分に構成されていない[アクセス許可スコープ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- [同意](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)がない

**_Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) のサポートの終了_* _

_*2020 年 6 月 30 日以降**、ADAL および Azure AD Graph に新しい機能は追加されなくなります。 テクニカル サポートおよびセキュリティ更新プログラムは引き続き提供されますが、機能の更新プログラムは提供されなくなります。

**2022 年 6月 30 日以降**、ADAL と Azure AD Graph のサポートは終了し、テクニカル サポートやセキュリティ更新プログラムは提供されなくなります。

既存の OS バージョンで ADAL を使用するアプリは、この期間以降も引き続き機能しますが、*テクニカル サポートやセキュリティ更新プログラムの提供* は行われません。

これ以降に Azure AD Graph を使用するアプリは、Azure AD Graph エンドポイントからの応答を受信しなくなる場合があります。

**ADAL 移行**

最新の機能とセキュリティ更新プログラムを備えた[Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) に更新することをお勧めします。

Microsoft アプリを使用している場合は、Microsoft がサポート終了期限までにアプリケーションを MSAL に移行していることを確認し、継続的に MSAL の強化されたセキュリティと機能を利用できるようにします。

1. [ADAL の FAQ を読む](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [プラットフォームごとにアプリを移行する方法に関する詳細情報](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. どのアプリが ADAL を使用しているかを理解するためにサポートが必要な場合は、すべてのアプリのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。 Microsoft サポートでは、テナントにあるすべての Microsoft ADAL 以外のアプリのリストも提供できます。

**AAD Graph の移行**

Azure AD Graph を使用しているアプリケーションの場合は、ガイダンスに従って [Azure AD Graph アプリを Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview) に移行してください。

1. [移行のチェックリストは、開始ポイントを提供します](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。
2. Azure アプリの登録ポータルには、AAD Graph を使用しているアプリケーションが表示されます。 アプリのすべてのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。 Microsoft のサポートでは、テナントでのすべての AAD Graph の使用状況のリストを提供することもできます。
3. アプリから Microsoft Graph のデータにアクセスする場合、ユーザーまたは管理者は、同意のプロセスを通してそのアプリに正しいアクセス許可を付与する必要があります。 [Microsoft Graph のアクセス許可リファレンス](https://docs.microsoft.com/graph/permissions-reference)では、Microsoft Graph API の各主要なセットに関連付けられているアクセス許可について説明します。 また、アクセス許可の使用方法に関するガイダンスを提供しています。

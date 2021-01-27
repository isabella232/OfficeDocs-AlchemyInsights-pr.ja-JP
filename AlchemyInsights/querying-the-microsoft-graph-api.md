---
title: Microsoft Graph API のクエリ
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975087"
---
# <a name="querying-the-microsoft-graph-api"></a>Microsoft Graph API のクエリ

このトピックは、Azure AD Graph API をまだ使用している開発者にも当てはまります。 ただし、すべてのディレクトリ、ID、およびアクセス管理シナリオで Microsoft Graph を使用することを **強く** お勧めします。

**認証または許可に関する問題**

- アプリが Microsoft Graph を呼び出すための **トークンを取得できない** 場合、**アクセス トークンの取得に関する問題 (認証)** Microsoft Graph カテゴリを選択して、このトピックに関するより具体的なヘルプとサポートを受けることができます。
- Microsoft Graph を呼び出しているときにアプリが **401 または 403 の認証エラー** を受信している場合は、**アクセス拒否エラー (認証)** Microsoft Graph API カテゴリを選択すると、このトピックに関するより具体的なヘルプとサポートを受けることができます。

**Microsoft Graph を使用したいが、開始点がわかりません**

Microsoft Graph の詳細については、以下を参照してください。

- [Microsoft Graph の概要](https://docs.microsoft.com/graph/overview)
- [Microsoft Graph の ID およびアクセス管理の概要](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph アプリの作成の開始](https://docs.microsoft.com/graph/)
- **Microsoft Graph エクスプローラー** - テナントまたはデモ テナントで Microsoft Graph API をテストする

**Microsoft Graph を使用したいが、必要な v1.0 ディレクトリ API をサポートしていますか?**

Microsoft Graph は、ディレクトリ、ID、およびアクセス管理に推奨される API です。 しかし、Azure AD Graph と Microsoft Graph にはまだいくつかのギャップがあります。 次の記事を確認してください。これらの記事では、選択に役立つ最新の違いを強調しています。

- [Azure AD Graph と Microsoft Graph のリソースの種類の違い](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graph と Microsoft Graph のプロパティの違い](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD と Microsoft Graph のメソッドの違い](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

***user* オブジェクトにクエリを実行すると、そのプロパティの多くが欠落します**

Microsoft Graph では *user* プロパティの既定のセットが自動的に選択されるため、`GET https://graph.microsoft.com/v1.0/users` は 11 プロパティだけを返します。 他の *user* プロパティが必要な場合は、$select を使用してアプリケーションに必要なプロパティを選択します。 まず **Microsoft Graph エクスプローラー** で試してください。

**一部の user プロパティ値は、設定されていても *null* です**

最も可能性の高い説明は、アプリケーションに *User.ReadBasic.All* アクセス許可が付与されていることです。 これにより、アプリケーションは限られた user プロパティ セットを読み取り、その他すべてのプロパティが以前に設定されていた場合でも null として返されます。 代わりに、アプリケーションに *User.Read.All* アクセス許可を付与してみます。

詳細については、「[Microsoft Graph の user アクセス許可](https://docs.microsoft.com/graph/permissions-reference#user-permissions)」を参照してください。

**OData クエリ パラメーターを使用して要求内のデータをフィルター処理できません**

Microsoft Graph は幅広い OData クエリー パラメーターをサポートしていますが、これらのパラメーターの多くは、Microsoft Graph のディレクトリ サービス (*directoryObject* から継承したリソース) では完全にはサポートされていません。 Azure AD Graph と同じ制限事項が Microsoft Graph の大部分で残っています。

1. **サポートなし**: *null* 値または *not null* 値に対する$count、$search、および $filter
2. **サポートなし**: 特定のプロパティの $filter on (プロパティがフィルター処理可能なリソースのトピックを参照）
3. **サポートなし**: ページング、フィルター処理、およびソートを同時に実行
4. **サポートなし**: 関係に基づくフィルター処理 たとえば、英国にあるすべてのエンジニアリング グループのメンバーを検索します。
5. **一部サポート**: *user* (displayName と userPrincipalName のみ) と *group* の $orderby
6. **一部サポート**: $filter (*eq*、*startswith*、*or*、*and* のみサポートし、*any* は制限) サポート、$expand (単一のオブジェクトの関係を展開するとすべての関係が返されるが、オブジェクトの関係のコレクションを展開すると制限あり)

詳細については、「[クエリ パラメーターを使用して応答をカスタマイズする](https://docs.microsoft.com/graph/query-parameters)」を参照してください。

**呼び出している API が機能しません。詳細なテストはどこで実行できますか?**

**Microsoft Graph エクスプローラー** - テナントまたはデモ テナントで Microsoft Graph API をテストし、Microsoft Graph エクスプローラーで **サンプル クエリ** を確認します。

**データをクエリすると、不完全なデータ セットが返されるようです**

コレクションをクエリする場合 (たとえば、*users*)、Microsoft Graph ではサーバー側のページ制限が使用されるため、結果は常に既定のページサイズで返されます。 アプリは常に、サービスから返されたコレクションをページングすることを期待する必要があります。

詳細については、以下を参照してください。

- [Microsoft Graph のベスト プラクティス](https://docs.microsoft.com/graph/best-practices-concept)
- [アプリの Microsoft Graph データをページングする](https://docs.microsoft.com/graph/paging)

**アプリは遅すぎて、制限もされています。改善する方法はありますか?**

シナリオに応じて、アプリケーションのパフォーマンスを向上させ、場合によっては、サービスによって制限される可能性を低くする (呼び出しが多すぎる場合) ために、さまざまなオプションを自由に使用できます。

詳細については、以下を参照してください。

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

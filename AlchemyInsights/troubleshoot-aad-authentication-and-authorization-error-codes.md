---
title: Azure AD Authentication と認証 (AADSTS) エラー コードのトラブルシューティング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038329"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Azure AD Authentication と認証 (AADSTS) エラー コードのトラブルシューティング

AAD 認証と承認エラー コード (AADSTS) を解決するには、次の推奨手順を実行します。

1. **アプリケーションでエラー コードを処理する**

- **OAuth2.0 仕様**、https://tools.ietf.org/html/rfc6749#section-5.2では、エラー応答のエラー部分を使用して、認証中にエラーを処理する方法を説明します。

    - **エラー**: 発生するエラーの種類を分類するために使用できるエラー コード文字列。エラーに対応するために使用する必要があります。
    - **エラー** フィールドにはいくつかの値が考えられる値があります。特定のエラーの詳細とそれに対応する方法の詳細については、プロトコル ドキュメントのリンクと OAuth 2.0 の仕様を確認してください。

- エラー応答の例を次に示します。
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **現在のエラー コードの情報を確認する**

- エラー コードとメッセージは変更される可能性があります。 最新の情報については、AADSTS エラーの説明、修正プログラム、およびいくつかの推奨される回避策について記載したhttps://login.microsoftonline.com/errorのページを参照してください。
- または、「[Azure AD Authentication と承認のエラー コード](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)」の記事に記載されている [AADSTS エラー コード](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes)を検索して、トラブルシューティングすることもできます。

3. **ヘルプを使用する**

- [開発者向けのサポートとヘルプのオプション](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - 質問に対する回答が欲しい場合、またはドキュメントに記載されていない問題を解決するための助けが必要な場合は、エキスパートにサポートを依頼することができます。 この記事では、Microsoft ID プラットフォームに統合するアプリの開発時に質問が発生した場合、どのようにしてそれに対する回答が得られるかについて、いくつかの提案を提供します。









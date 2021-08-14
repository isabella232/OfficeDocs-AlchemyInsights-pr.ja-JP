---
title: アプリケーション エラー
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931454"
---
# <a name="application-errors"></a>アプリケーション エラー

Azure Active Directory (Azure AD) セキュリティ トークン サービス (STS) から返される **AADSTS エラー コード** に関する情報をお探しですか? AADSTS エラーの説明、修正、およびいくつかの推奨される回避策については、「[Azure AD 認証および認証エラー コード](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)」を参照してください。

認証エラーは、いくつかの異なる問題の結果である可能性があり、そのほとんどは 401 または 403 エラーを生成します。 たとえば、次の場合はすべて承認エラーが発生する可能性があります。

- 間違った[アクセス トークンの取得フロー](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- 十分に構成されていない[アクセス許可スコープ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- [同意](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)がない

一般的な認証エラーを解決するには、発生しているエラーに最も近い以下の手順を試してください。 複数のエラーが適用される場合があります。

**401 Unauthorized エラー: トークンは有効ですか?**

アプリケーションが要求の一部として、Microsoft Graph への有効なアクセス トークンを提示していることを確認します。 このエラーは、多くの場合、HTTP 認証要求ヘッダーにアクセス トークンが存在しないか、トークンが無効であるか、有効期限が切れている可能性があることを意味します。 アクセス トークンの取得には、[Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) を使用することを強くお勧めします。 さらに、このエラーは、個人の Microsoft アカウントに付与されている代理アクセス トークンを使用して、職場または学校のアカウント (組織のアカウント) のみをサポートする API にアクセスしようとする場合に発生することがあります。

**403 Forbidden エラー: 適切なアクセス許可のセットを選択しましたか?**

アプリが呼び出す Microsoft Graph API に基づいて、適切なアクセス許可のセットを要求したことを確認します。 推奨される最小特権アクセス許可は、Microsoft Graph API リファレンス メソッドのすべてのトピックで提供されます。 また、これらのアクセス許可は、ユーザーまたは管理者がアプリケーションに付与する必要があります。 通常、アクセス許可の付与は、同意ページを経由するか、Azure Portal アプリケーションの登録ブレードを使用してアクセス許可を付与することによって行われます。 アプリケーションの [**設定**] ブレードで、[**必要なアクセス許可**] をクリックして、[**アクセス許可の付与**] をクリックします。

- [Microsoft Graph のアクセス許可](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD のアクセス許可と同意を理解する](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Forbidden エラー: アプリは選択されたアクセス許可と一致するトークンを取得しましたか?**

要求されたアクセス許可または与えられたアクセス許可の種類が、アプリが取得すアクセス トークンの種類と一致することを確認します。 アプリケーションのアクセス許可を要求して付与しますが、クライアント資格情報フロー トークンの代わりに、委任された対話型コード フロー トークンを使用する可能性があります。また、委任されたアクセス許可を要求して付与しますが、委任されたコード フロー トークンの代わりに、クライアント資格情報フロートークンを使用する可能性があります。

- [ユーザーに代わってアクセス権を取得し、アクセス許可を委任する](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - OAuth 2.0 承認コード フロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [ユーザー (デーモン サービス) とアプリケーションのアクセス許可なしでアクセス権を取得する](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - OAuth 2.0 クライアント資格情報フロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Forbidden エラー: パスワードの再設定**

現在、ユーザー パスワードの再設定を許可するアプリケーションのアクセス許可デーモンサービス間のアクセス許可はありません。 これらの API は、サインインしている管理者による対話型の委任されたコード フローを使用する場合にのみサポートされます。

- [Microsoft Graph のアクセス許可](https://docs.microsoft.com/graph/permissions-reference)

**403不可: ユーザーにアクセス権があり、ライセンスが付与されていますか?**

委任されたコード フローの場合、Microsoft Graph は、アプリに付与されたアクセス許可とサインインしたユーザーが持つアクセス許可に基づいて、要求が許可されているかどうかを評価します。 一般に、このエラーは、アクセスされているデータに対してユーザーにライセンスが付与されていない要求  または  を実行するための十分な特権がユーザーにないことを示しています。 必要なアクセス許可またはライセンスを持つユーザーのみが要求を正常に行うことができます。

**403 Forbidden: 正しいリソース API を選択しましたか?**

Microsoft Graph などの API サービスは、受信したアクセス トークンの aud クレーム (オーディエンス) が、それ自体が予期する値と一致することを確認します。一致しない場合は、403 Forbidden エラーとなります。 このエラーの原因となる一般的な間違いは、Azure AD Graph API、Outlook API、または SharePoint/OneDrive API で取得したトークンを使用して Microsoft Graph を呼び出すことです (またはその逆)。 アプリがトークンを取得しているリソース (またはスコープ) が、アプリが呼び出している API と一致していることを確認してください。

**400 要求が正しくありませんまたは 403 Forbidden: ユーザーは組織の条件付きアクセス (CA) ポリシーに準拠していますか?**

組織の CA ポリシーに基づいて、アプリを使用して Microsoft Graph リソースにアクセスするユーザーは、アプリが最初に取得したアクセス トークンに存在しない追加情報を要求される場合があります。 この場合、アプリはアクセス トークンの取得中に *interaction_required* エラーと共に 400 を受け取り、Microsoft Graph を呼び出すときに *insufficient_claims* エラーと共に 403 を受け取ります。 どちらの場合も、エラー応答には、承認エンドポイントに提示して、ユーザーに追加情報 (多要素認証やデバイス登録など) を要求できる追加情報が含まれます。

- [MSAL を使用して、条件付きアクセスの課題を処理する](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Azure Active Directory 条件付きアクセスの開発者ガイダンス](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)

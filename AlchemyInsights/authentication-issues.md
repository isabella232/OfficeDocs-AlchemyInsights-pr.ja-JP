---
title: 認証に関する問題点
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976854"
---
# <a name="authentication-issues"></a>認証に関する問題点

**Azure Active Directory (Azure AD) セキュリティ トークン サービス (STS) から返される AADSTS エラー コードに関する情報をお探しですか?** AADSTS エラーの説明、修正、およびいくつかの推奨される回避策については、「[Azure AD 認証および認証エラー コード](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)」を参照してください。

認証エラーは、いくつかの異なる問題の結果である可能性があり、そのほとんどは 401 または 403 エラーを生成します。 たとえば、次の問題はすべて認証エラーが発生する可能性があります。

- 間違った[アクセス トークンの取得フロー](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- 十分に構成されていない[アクセス許可スコープ](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- [同意](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)がない

一般的な認証エラーを解決するには、発生しているエラーに最も近い以下の手順を試してください。 発生したエラーには、複数の手順が適用される場合があります。

**401 Unauthorized エラー: トークンは有効ですか?**

アプリが要求の一部として、Microsoft Graph への有効なアクセス トークンを提示していることを確認します。 このエラーは、多くの場合、HTTP 認証要求ヘッダーにアクセス トークンが存在しないか、トークンが無効であるか、有効期限が切れている可能性があることを意味します。 アクセス トークンの取得には、Microsoft Authentication Library (MSAL) を使用することを強くお勧めします。 さらに、このエラーは、個人の Microsoft アカウントに付与されている代理アクセス トークンを使用して、職場または学校のアカウント (組織のアカウント) のみをサポートする API にアクセスしようとする場合に発生することがあります。

**403 Forbidden エラー: 適切なアクセス許可のセットを選択しましたか?**

アプリが呼び出す Microsoft Graph API に基づいて、適切なアクセス許可のセットを要求したことを確認します。 推奨される最小特権アクセス許可は、Microsoft Graph API リファレンス メソッドのすべてのトピックで提供されます。 また、これらのアクセス許可は、ユーザーまたは管理者がアプリケーションに付与する必要があります。 通常、アクセス許可の付与は、同意ページまたは Azure Portal アプリケーションの登録ブレードの使用を通じて行われます。 アプリケーションの **[設定]** ブレードで、**[必要なアクセス許可]** をクリックして、**[アクセス許可の付与]** をクリックします。 詳しくは、以下を参照してください。

- [Microsoft Graph のアクセス許可](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD のアクセス許可と同意を理解する](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Forbidden エラー: アプリは選択されたアクセス許可と一致するトークンを取得しましたか?**

要求されたアクセス許可の種類または与えられたアクセス許可の種類が、アプリが取得すアクセス トークンの種類と一致することを確認します。 アプリのアクセス許可を要求して付与しますが、クライアント資格情報フロー トークンの代わりに、委任された対話型コード フロー トークンを使用する可能性があります。また、委任されたアクセス許可を要求して付与しますが、委任されたコード フロー トークンの代わりに、クライアント資格情報フロー トークンを使用する可能性があります。

トークンの取得に関する詳細については、以下を参照してください。

- [ユーザーに代わってアクセス権を取得し、アクセス許可を委任する](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - OAuth 2.0 承認コード フロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [ユーザー (デーモン サービス) とアプリケーションのアクセス許可なしでアクセス権を取得する](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - OAuth 2.0 クライアント資格情報フロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Forbidden エラー: パスワードの再設定**

現在、ユーザー パスワードの再設定を許可するアプリケーションのアクセス許可デーモンサービス間のアクセス許可はありません。 これらの API は、サインインしている管理者による対話型の委任されたコード フローを使用する場合にのみサポートされます。 詳細については、「[Microsoft Graph のアクセス許可](https://docs.microsoft.com/graph/permissions-reference)」を参照してください。

**403 Forbidden: ユーザーにアクセス権があり、ライセンスが付与されていますか?**

委任されたコード フローの場合、Microsoft Graph は、アプリに付与されたアクセス許可とサインインしたユーザーが持つアクセス許可に基づいて、要求が許可されているかどうかを評価します。 一般に、このエラーは、アクセスされているデータに対してユーザーにライセンスが付与されていない要求 **または** を実行するための十分な特権がユーザーにないことを示しています。 必要なアクセス許可またはライセンスを持つユーザーのみが要求を正常に行うことができます。

**403 Forbidden: 正しいリソース API を選択しましたか?**

Microsoft Graph などの API サービスは、受信したアクセス トークンの *および* クレーム (オーディエンス) が、それ自体が予期する値と一致することを確認します。一致しない場合は、403 Forbidden エラーが発生します。 このエラーの原因となる一般的な間違いは、Azure AD Graph API、Outlook API、または SharePoint/OneDrive API で取得したトークンを使用して Microsoft Graph を呼び出すことです (またはその逆)。 アプリがトークンを取得しているリソース (またはスコープ) が、アプリが呼び出している API と一致していることを確認してください。

**400 要求が正しくありませんまたは 403 Forbidden: ユーザーは組織の条件付きアクセス (CA) ポリシーに準拠していますか?**

組織の条件付きアクセス (CA) ポリシーに基づいて、アプリを使用して Microsoft Graph リソースにアクセスするユーザーは、アプリが最初に取得したアクセス トークンに存在しない追加情報を要求される場合があります。 この場合、アプリはアクセス トークンの取得中に **400 と *interaction_required*** エラーを受け取り、Microsoft Graph を呼び出すときに **403 と *insufficient_claims*** エラーを受け取ります。 どちらの場合も、エラー応答には、認証エンドポイントに提示して、ユーザーに追加情報 (多要素認証やデバイス登録など) を要求できる追加情報が含まれます。

条件付きアクセスに関する詳細については、以下を参照してください。

- [MSAL を使用して、条件付きアクセスの課題を処理する](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Azure Active Directory 条件付きアクセスの開発者ガイダンス](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) のサポートの終了_* _

- 2020 年 6 月 30 日以降、Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) に新しい機能を追加しなくなります。 テクニカル サポートおよびセキュリティ更新プログラムは引き続き提供されますが、機能の更新プログラムは提供されなくなります。
- 2022 年 6月 30 日に ADAL および AAD Graph のサポートは終了し、以降はテクニカル サポートやセキュリティ更新プログラムは提供されなくなります。
    - 既存の OS バージョンで ADAL を使用するアプリは、この期間以降も引き続き機能しますが、テクニカル サポートやセキュリティ更新プログラムは提供されません。
    - これ以降に AAD Graph を使用するアプリは、AAD Graph エンドポイントからの応答を受信しなくなる場合があります。

_ *ADAL 移行**

最新の機能とセキュリティ更新プログラムを備えた[Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) に更新することをお勧めします。 この推奨事項は、Microsoft がサポート終了期限までにアプリケーションを MSAL に移行することに関連しています。 Microsoft アプリを MSAL に移行する目的は、アプリが継続的に MSAL の強化されたセキュリティと機能を利用できることを保証するためです。

- [ADAL の FAQ を読む](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [プラットフォームごとにアプリを移行する方法に関する詳細情報](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- どのアプリが ADAL を使用しているかを理解するためにサポートが必要な場合は、すべてのアプリのソース コードを確認し、該当する場合は、独立系ソフトウェア ベンダー (ISV) またはアプリ プロバイダーに連絡することをお勧めします。 Microsoft サポートでは、テナントにあるすべての Microsoft ADAL 以外のアプリのリストも提供できます。

**AAD Graph の移行**

AAD Graph を使用しているアプリケーションの場合は、ガイダンスに従って [Azure AD Graph アプリを Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true) に移行してください。

- [移行のチェックリストは、開始ポイントを提供します](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。 
- Azure アプリの登録ポータルには、AAD Graph を使用しているアプリケーションが表示されます。 アプリのすべてのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。 Microsoft のサポートでは、テナントでのすべての AAD Graph の使用状況に関する情報を提供することもできます。

 











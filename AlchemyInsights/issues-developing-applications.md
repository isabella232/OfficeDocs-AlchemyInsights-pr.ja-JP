---
title: アプリケーションの開発に関する問題
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
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975094"
---
# <a name="issues-developing-applications"></a>アプリケーションの開発に関する問題

Azure Active Directory (AD) アプリを作成するときに発生する最も一般的な問題のトラブルシューティングを行うには、次の記事を参照してください。

- [Chrome ブラウザーのみを使用してアプリケーションにサインインする際に問題が発生します](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [アプリケーションのトークンの有効期間の既定値を変更する方法がわかりません](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [アプリケーションの同意の仕組みに混乱しています](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [アプリケーションにアクセス許可を付与する方法がわかりません](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [委任されたアクセス許可とアプリケーションのアクセス許可の違いがわかりません](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) のサポートの終了** _

- 2020 年 6 月 30 日以降、Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) に新しい機能を追加しなくなります。 テクニカル サポートおよびセキュリティ更新プログラムは引き続き提供されますが、機能の更新プログラムは提供されなくなります。

- 2022 年 6月 30 日に ADAL および AAD Graph のサポートは終了し、以降はテクニカル サポートやセキュリティ更新プログラムは提供されなくなります。 この条件の結果、次のような影響があります。

    - 既存の OS バージョンで ADAL を使用するアプリは、この期間以降も引き続き機能しますが、テクニカル サポートやセキュリティ更新プログラムは提供されません。

    - これ以降に AAD Graph を使用するアプリは、AAD Graph エンドポイントからの応答を受信しなくなる場合があります

_ *ADAL 移行**

Microsoft アプリを使用している場合、最新の機能とセキュリティ更新プログラムを備えた Microsoft Authentication Library (MSAL) に更新することをお勧めします。 この推奨事項は、Microsoft がサポート終了期限までにアプリを MSAL に移行するプロセスを開始することに関連しています。 

Microsoft アプリを MSAL に移行すると、アプリが継続的に MSAL の強化されたセキュリティと機能を利用できます。

1. [ADAL の FAQ を読む](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [プラットフォームごとにアプリを移行する方法に関する詳細情報](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. どのアプリが ADAL を使用しているかを理解するためにサポートが必要な場合は、すべてのアプリのソース コードを確認し、該当する場合は、独立系ソフトウェア ベンダー (ISV) またはアプリ プロバイダーに連絡することをお勧めします。 Microsoft サポートでは、テナントにあるすべての Microsoft ADAL 以外のアプリのリストも提供できます。

**AAD Graph の移行**

AAD Graph を使用しているアプリケーションの場合は、ガイダンスに従って AAD Graph アプリを Microsoft Graph に移行してください。

1. [移行のチェックリストは、開始ポイントを提供します](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。 
2. Azure アプリの登録ポータルには、AAD Graph を使用しているアプリケーションが表示されます。 アプリのすべてのソース コードを確認し、該当する場合は、独立系ソフトウェア ベンダー (ISV) またはアプリ プロバイダーに連絡することをお勧めします。 Microsoft のサポートでは、テナントでの AAD Graph の使用状況に関する情報を提供することもできます。








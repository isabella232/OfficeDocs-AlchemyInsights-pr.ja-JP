---
title: 認証ライブラリの操作
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038238"
---
# <a name="working-with-authentication-libraries"></a>認証ライブラリの操作

Microsoft 認証ライブラリ (MSAL) の問題を解決するには、次の推奨手順を実行します。

1. **MSAL の操作**: [Microsoft ID プラットフォーム認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - この記事では、複数のアプリケーションの種類に対する Microsoft 認証ライブラリのサポートについて説明します。 これには、ライブラリのソース コードへのリンク、アプリのプロジェクトのパッケージを取得する場所を含み、ライブラリがユーザーのサインイン(認証)か、保護された Web API へのアクセス (承認)をサポートするのかどうか、あるいはその両方がサポートされているのかを確認できます。

2. **トラブルシューティング認証**: MSAL は、さまざまなアプリケーション シナリオで使用する複数の認証フローをサポートしています。 クライアント アプリケーションの構築方法によっては、MSAL は Microsoft ID プラットフォームでサポートされる 1 つ以上の認証フローを使用できます。 これらのフローは、いくつかの種類のトークンおよび承認コードを生成する可能性があり、それらを動作させるためには、異なるトークンが必要です。

3. **アクセス トークン**: 「[Microsoft ID プラットフォームのアクセス トークン](https://docs.microsoft.com/azure/active-directory/develop/access-tokens)」 - API がアクセス トークン内のクレームを検証および使用する方法を参照してください。 特に明示されている場合を除き、この記事のすべてのドキュメントは、登録した API に対して発行されるトークンにのみ適用されます。 これは、Microsoft 所有の API で発行されるトークンには適用されません。また、これらのトークンを使用して、作成した API に対して Microsoft ID プラットフォームがトークンを発行する方法を検証することもできません。

**Azure Active Directory 認証ライブラリ (ADAL) のサポートが終了しました**

- **2020 年 6 月 30 日以降、** ADAL および Azure AD Graph に新しい機能は追加されなくなります。 テクニカル サポートおよびセキュリティ更新プログラムは引き続き提供されますが、機能の更新プログラムは提供されなくなります。
- **2022 年 6月 30 日以降、** ADAL および Azure AD Graph のサポートは終了し、テクニカル サポートやセキュリティ更新プログラムは提供されなくなります。
- 既存の OS バージョンで ADAL を使用するアプリは、この期間以降も引き続き機能しますが、*テクニカル サポートやセキュリティ更新プログラムの提供* は行われません。
- これ以降に Azure AD Graph を使用するアプリは、Azure AD Graph エンドポイントからの応答を受信しなくなる場合があります。

**ADAL 移行**

- 最新の機能とセキュリティ更新プログラムを備えた MSAL に更新することをお勧めします。
- Microsoft アプリを使用している場合は、Microsoft がサポート終了期限までにアプリを MSAL に移行していることを確認し、継続的に MSAL の強化されたセキュリティと機能を利用できるようにします。

1. [ADAL の FAQ を確認します](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。
2. [プラットフォームごとにアプリを移行する方法について説明します](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)。
3. アプリのプラットフォームのガイドを読んだ後、他にも質問がある場合は、[azure-ad-adal-deprecation] タグを使って、「[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html)」 に投稿するか、ライブラリの GitHub リポジトリで問題を開くことができます。 各ライブラリのリポジトリへのリンクについては、**MSAL の概要** 記事の、「[言語とフレームワーク](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks)」セクションを参照してください。
4. **どのアプリが ADAL を使用しているかを理解するためにサポートが必要な場合は**、すべてのアプリのソース コードを確認することをお勧めします。 該当する場合は、独立系ソフトウェア ベンダー (ISV) またはアプリ プロバイダーに問い合わせください。 Microsoft サポートでは、テナントにあるすべての Microsoft ADAL 以外のアプリのリストも提供できます。








---
title: アプリケーションの構成とカスタマイズ
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063732"
---
# <a name="configure-and-customize-applications"></a>アプリケーションの構成とカスタマイズ

**アプリケーションの構成**

1. 「[クイックスタート: Azure Active Directory (Azure AD) テナントでアプリケーションのプロパティを構成する](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)」は、アプリのいくつかのプロパティを構成する方法を示しています。
2. アプリケーションを Azure Active Directory と統合するために、構成の手順を説明する[一連のチュートリアル](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)を開発しました。
3. 「[アプリケーション プロキシ アプリケーションの構成方法](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to)」は、オンプレミス アプリケーションをクラウドに公開するように Azure AD 内でアプリケーション プロキシ アプリケーションを設定する方法を理解するのに役立ちます。
4. [PingAccess のダウンロードとアプリケーションの構成](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): Ping Identity Web サイトで Microsoft Azure AD アプリケーション プロキシを使用して公開された「*Azure AD 用に PingAccess を構成してアプリケーションを保護する*」の手順に従い、最新バージョンの PingAccess をダウンロードします。

**正しく構成されなかったアプリケーション (AADS650056) エラー**

1. アプリケーション所有者から提供されたサインイン アドレスからアプリケーションにアクセスしていることを確認します。 それ以外の場合は、通常のプロセスでアプリケーションにサインインします。 ほとんどの場合、これは自動的に解決されます。 問題が解決しない場合は、この投稿がトラブルシューティングおよび解決に役立ちます。
2. **組織がアプリケーションを所有している場合** (アプリケーション登録が組織内にあることを意味します):
    - 少なくとも、**Microsoft Graph** から委任された `User.Read` または `openid` のアクセス許可を追加することをお勧めします。
    - アプリケーションとそのすべてのアクセス許可が同意されていることを確認します。 これを確認するには、**API アクセス許可** 内のアプリケーション登録の **[状態]** を参照してください。
    - 場合によっては、アプリケーションがサードパーティ製であっても、組織に登録されている可能性があります。 このアプリケーションがアプリ登録に一覧表示されているかどうかを確認します (エンタープライズ アプリケーションではありません) 。
    - このエラー メッセージが引き続き表示される場合は、 **手順 4** で説明されている同意 URL を作成する必要があります。
3. **組織がアプリケーションの所有者ではなく、アプリケーションをサードパーティ アプリケーションとして使用している場合**:
    - グローバル/社内管理者の場合は、同意画面が表示されます。 **「組織の代理として同意する」** のチェックボックスをオンにしてください。
    - 同意画面が表示されない場合は、エンタープライズ アプリケーションを削除してから、もう一度お試しください。
    - このエラー メッセージが引き続き表示される場合は、 **手順 4** で説明されている同意 URL を作成する必要があります。
4. **使用する同意 URL を手動で構築する**: アプリケーションが特定のリソースにアクセスするように設計されている場合、Azure portal, から [同意] ボタンを使用できないことがあります。独自の同意 URL を手動で生成して使用する必要があります。
    - アプリケーションの所有者から `{App-Id}` と `{App-Uri-Id}` を取得する必要があります。 `{Tenant-Id}` はテナント識別子になります。 これは、`yourdomain.onmicrosoft.com` またはディレクトリ ID のいずれかになります。
    - アプリケーションがリソースに対して自身にアクセスしている場合、`{App-Id}` と `{App-Uri-Id}` は同じになります。
5. 詳細については、「[SAML ベースのシングル サインオンで構成されたアプリへのサインインに関する問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)」を参照してください。

**アプリケーションのカスタマイズ**

- [組織の Azure Active Directory サインイン ページにブランドを追加する](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) - 組織のロゴとユーザー設定の配色パターンを使用して、Azure Active Directory (Azure AD) サインイン ページに一貫した外観を提供します。
- [Azure Active Directory ポータルを使用してカスタム ドメイン名を追加する](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) - すべての新しい Azure AD テナントには、初期ドメイン名が付いています。 初期ドメイン名は変更または削除できませんが、組織名は追加できます。 カスタム ドメイン名を追加すると、ユーザーになじみのあるユーザー名を作成できます。

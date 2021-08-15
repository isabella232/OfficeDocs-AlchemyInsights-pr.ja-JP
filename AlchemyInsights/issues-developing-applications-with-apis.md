---
title: API を使用したアプリケーションの開発に関する問題
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
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013465"
---
# <a name="issues-developing-applications-with-apis"></a>API を使用したアプリケーションの開発に関する問題

Azure Active Directory Graph API の使用を開始するには、「[Azure AD Graph API クイック スタート ガイド](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro)」を参照するか、「[対話型の Azure AD Graph API リファレンス ドキュメント](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)」を表示します。

**Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) のサポートの終了** _

**2020 年 6 月 30 日以降**、ADAL および Azure AD Graph に新しい機能は追加されなくなります。 テクニカル サポートおよびセキュリティ更新プログラムは引き続き提供されますが、機能の更新プログラムは提供されなくなります。

**2022 年 6月 30 日以降**、ADAL と Azure AD Graph のサポートは終了し、テクニカル サポートやセキュリティ更新プログラムは提供されなくなります。

既存の OS バージョンで ADAL を使用するアプリは、この期間以降も引き続き機能しますが、テクニカル サポートやセキュリティ更新プログラムは提供されません。

これ以降に Azure AD Graph を使用するアプリは、Azure AD Graph エンドポイントからの応答を受信しなくなる場合があります。

**ADAL 移行**

最新の機能とセキュリティ更新プログラムを備えた[Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) に更新することをお勧めします。

Microsoft アプリを使用している場合は、Microsoft がサポート終了期限までにアプリケーションを MSAL に移行していることを確認し、継続的に MSAL の強化されたセキュリティと機能を利用できるようにします。

1. [ADAL の FAQ を確認します](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。
1. [プラットフォームごとにアプリを移行する方法について説明します](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。
1. どのアプリが ADAL を使用しているかを理解するためにサポートが必要な場合は、すべてのアプリのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。 Microsoft サポートでは、テナントにあるすべての Microsoft ADAL 以外のアプリのリストも提供できます。

**AAD Graph の移行**

Azure AD Graph を使用しているアプリケーションの場合は、ガイダンスに従って [Azure AD Graph アプリを Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true) に移行してください。

1. [移行のチェックリストは、開始ポイントを提供します](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。 
1. Azure アプリの登録ポータルには、AAD Graph を使用しているアプリケーションが表示されます。 アプリのすべてのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。 Microsoft のサポートでは、テナントでのすべての AAD Graph の使用状況のリストを提供することもできます。
1. アプリから Microsoft Graph のデータにアクセスする場合、ユーザーまたは管理者は、同意のプロセスを通してそのアプリに正しいアクセス許可を付与する必要があります。 [Microsoft Graph のアクセス許可リファレンス](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true)では、Microsoft Graph API の各主要なセットに関連付けられているアクセス許可について説明します。 また、アクセス許可の使用方法に関するガイダンスを提供しています。

---
title: API アクセス許可と同意の手順
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405827"
---
# <a name="api-permissions-and-consent-process"></a>API アクセス許可と同意の手順

アプリから Microsoft Graph のデータにアクセスする場合、ユーザーまたは管理者は、同意のプロセスを通してそのアプリに正しいアクセス許可を付与する必要があります。 [Microsoft Graph のアクセス許可リファレンス](https://docs.microsoft.com/graph/permissions-reference)では、Microsoft Graph API の各主要なセットに関連付けられているアクセス許可について説明します。 また、アクセス許可の使用方法に関するガイダンスを提供しています。

**サービス プリンシパルを設定または更新する**

- [serviceprincipal の作成](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - この記事では、新しい servicePrincipal オブジェクトを作成する方法を説明します。
- [ポータルを使用して Azure AD アプリとサービス プリンシパルを作成する](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - この記事では、役割ベースのアクセス制御で使用できる新しい Azure Active Directory (Azure AD) アプリケーションとサービス プリンシパルを作成する方法が示されています。
- [AzureAD のアプリとサービスプリンシパル](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - この記事では、Azure Active Directory でのアプリケーションの登録、アプリケーション オブジェクト、およびサービス プリンシパルについて、それらが何であるか、どのように使用されるか、お互いがどのように関連しているかについて説明しています。

**アプリ登録を追加または更新し、管理者の同意を提供します**

- [アプリ登録の作成](https://docs.microsoft.com/graph/api/application-post-applications) - この記事では、新しいアプリケーション オブジェクトを作成する方法を説明します。
- [アプリ登録の更新 - API 権限](https://docs.microsoft.com/graph/api/application-update) - この記事では、アプリケーション オブジェクトのプロパティを更新する方法を説明します。
- [管理者の同意を提供する](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - 管理者の同意と一般的な同意については、管理者が明示的に同意を与える必要があります。
- [RBAC (ベータ版)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - 単一の役割割り当てで複数のプリンシパルと複数の範囲をサポートする Microsoft 365 RBAC プロバイダーの統合された役割定義と役割割り当てのための役割管理コンテナー。 これは、*rbacApplication* リソース タイプとは異なります。 Microsoft Intune は、そのような RBAC プロバイダーの一例です。 Intune での役割の割り当てには、プリンシパルの配列と範囲グループの配列を含めることができます。 **これはベータ版です。つまり、まだ開発中であり、本番環境での使用は推奨されていません。**

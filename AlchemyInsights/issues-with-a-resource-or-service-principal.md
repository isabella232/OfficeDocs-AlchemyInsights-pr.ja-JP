---
title: リソースまたはサービス プリンシパルに関する問題
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/28/2021
ms.locfileid: "50035755"
---
# <a name="issues-with-a-resource-or-service-principal"></a>リソースまたはサービス プリンシパルに関する問題

1. まだ使用を開始したばかりのユーザーには、「[Azure Active Directory のアプリケーション オブジェクトとサービス プリンシパル オブジェクト](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)」で、Azure Active Directory でのアプリケーションの登録、アプリケーション オブジェクト、およびサービス プリンシパルについて、それらが何であるか、どのように使用されるか、お互いがどのように関連しているかについて説明しています。 また、アプリケーションのアプリケーション オブジェクトと対応するサービス プリンシパル オブジェクトとの関係を説明するために、マルチテナントのサンプル シナリオが提示されています。
2. アプリケーションとサービス プリンシパルの関係の詳細については、「[Azure Active Directory のアプリケーションとサービス プリンシパル オブジェクト](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)」をお読みください。
3. 「[方法: ポータルを使用して、リソースにアクセスできる Azure AD アプリケーションとサービス プリンシパルを作成する](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)」では、役割ベースのアクセス制御で使用できる新しい Azure Active Directory (Azure AD) アプリケーションとサービス プリンシパルを作成する方法が示されています。
4. [サービス プリンシパル API](https://docs.microsoft.com/graph/api/resources/serviceprincipal) を使用すると、アプリケーションのインスタンスをプログラムで管理し、テナント内でアプリケーションが実行できることを制御できます。
5. 「[servicePrincipal リソースの種類](https://docs.microsoft.com/graph/api/resources/serviceprincipal)」では、servicePrincipal リソースの種類のすべてのプロパティとメソッドが一覧表示されています。
6. 「[Azure AD Graph と Microsoft Graph のリソースの種類の違い](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)」では、Azure AD Graph と Microsoft Graph リソースの違いに焦点を当てています。 異なる名前を持つリソースや、利用できないリソースを紹介し、また、Microsoft Graph のベータ版では利用できるものの、v1.0 バージョンでは利用できないリソースにも焦点を当てています。

**ゲスト ユーザーに関する問題**

- 「[クイックスタート: Azure portal のディレクトリにゲストユーザーを追加する](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites)」では、Azure portal を介して新しいゲストユーザーを Azure AD ディレクトリに追加し、招待状を送信し、ゲスト ユーザーの招待状の引き換えプロセスがどのようになるかを確認する方法が示されています。
- 「[チュートリアル: Azure Active Directory B2C でユーザー フローを作成する](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows)」では、Azure portal を使用して、いくつかの推奨ユーザー フローを作成する方法を示しています。 アプリケーションでリソース所有者のパスワード資格情報 (ROPC) フローをセットアップする方法については、「Configure the resource owner password credentials flow in Azure AD B2C (Azure AD B2C でリソース所有者のパスワード資格情報フローを構成する)」を参照してください。

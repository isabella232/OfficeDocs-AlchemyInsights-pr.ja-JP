---
title: エンタープライズ アプリケーションのリストを取得する
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405834"
---
# <a name="get-a-list-of-enterprise-applications"></a>エンタープライズ アプリケーションのリストを取得する

1. Powershell コマンドを使用して **エンタープライズ アプリケーション (すべてのアプリケーションまたは表示名、ID、識別子 URI などでフィルター処理されたもの) のリストを取得する** には、[Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication) を参照してください。
2. Powershell コマンドを使用してサービス プリンシパル オブジェクト (すべてのオブジェクトまたは ID でフィルター処理されたオブジェクト) のリストを取得するには、[Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal) を参照してください。
3. **SAML で構成されたアプリのリストを取得する** 場合は、次の PowerShell スクリプトが役立ちます。

    OAuth アプリまたは SAML アプリ (ギャラリー アプリと非ギャラリー アプリの両方) のすべてのアプリケーションには、登録時に AAD で作成された 2 つのオブジェクトがあります。 1 つはアプリケーション オブジェクトと呼ばれ、もう 1 つはサービス プリンシパル オブジェクトと呼ばれます。 PowerShell を使用してサービス プリンシパル オブジェクトのプロパティをダンプすると、すべてのアプリケーションに次のような特定の数のタグが関連付けられていることがわかります。

    - OAuthアプリには、"**WindowsAzureActiveDirectoryIntegratedApp**" というタグがあります。
    - Gallery SAML Appsには、"**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**" というタグがあります。
    - 非ギャラリー SAML アプリには、"**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**" というタグがあります。

    したがって、これらのタグを使用して、それがどのようなアプリであるかを調べることができます。 タグ "**WindowsAzureActiveDirectoryIntegratedApp**" は、すべての種類のアプリに共通です。 次のスニペットを使用して、すべての SAML アプリ (ギャラリーと非ギャラリーの両方) を一覧表示できます。

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    詳細については、「[AzureAD で SAML 対応アプリを特定する](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)」を参照してください。

4. **Web アプリケーションのみを検索して一覧表示する**: 以下のコマンドを使用して、アプリケーション タイプが "Web app/API" のすべての AzureAD アプリケーションを取得します。

    Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT
5. **ネイティブ アプリケーションのみを検索して一覧表示する**: 次のコマンドを実行して、すべてのネイティブ クライアント (デスクトップ/モバイルデバイス) アプリケーションを取得します。

    Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT
6. **登録されているすべての AzureAD アプリケーションの詳細を CSV にエクスポートする**: 次のコマンドは、必要な詳細を含むすべての AzureAD アプリを csv ファイルにエクスポートします。

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **未使用の Azure アプリのリストをエクスポートする必要がある** – 監査レポート

    Azure AD Premium ライセンスを持っている場合、Azure AD は最大 30 日間のみアプリケーション ログを表示できます。
    30 日を超えてデータを保持するための 2 つのオプションがあります。 [Azure AD Reporting API](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) を使用して、プログラムでデータを取得し、データベースに保存できます。 または、監査ログをサード パーティの SIEM システムに統合することもできます。

    [Azure ActiveDirectory] > [アプリ登録] > [ダウンロード] > [すべてのアプリケーション/所有アプリケーション] からすべてのアプリケーションと所有アプリケーションのアプリ リストをダウンロードすることもできます。

    MS Graph を介してアプリケーションのリストを取得するには、「[アプリケーションを一覧表示する - Microsoft Graphv1.0](https://docs.microsoft.com/graph/api/application-list)」および「[アプリケーション リソース タイプ - MicrosoftGraphv1.0](https://docs.microsoft.com/graph/api/resources/application)」を参照してください。

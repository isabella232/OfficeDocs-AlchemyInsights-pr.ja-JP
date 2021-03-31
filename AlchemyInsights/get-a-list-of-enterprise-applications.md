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
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="5f5b5-102">エンタープライズ アプリケーションのリストを取得する</span><span class="sxs-lookup"><span data-stu-id="5f5b5-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="5f5b5-103">Powershell コマンドを使用して **エンタープライズ アプリケーション (すべてのアプリケーションまたは表示名、ID、識別子 URI などでフィルター処理されたもの) のリストを取得する** には、[Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="5f5b5-104">Powershell コマンドを使用してサービス プリンシパル オブジェクト (すべてのオブジェクトまたは ID でフィルター処理されたオブジェクト) のリストを取得するには、[Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="5f5b5-105">**SAML で構成されたアプリのリストを取得する** 場合は、次の PowerShell スクリプトが役立ちます。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="5f5b5-106">OAuth アプリまたは SAML アプリ (ギャラリー アプリと非ギャラリー アプリの両方) のすべてのアプリケーションには、登録時に AAD で作成された 2 つのオブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="5f5b5-107">1 つはアプリケーション オブジェクトと呼ばれ、もう 1 つはサービス プリンシパル オブジェクトと呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="5f5b5-108">PowerShell を使用してサービス プリンシパル オブジェクトのプロパティをダンプすると、すべてのアプリケーションに次のような特定の数のタグが関連付けられていることがわかります。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="5f5b5-109">OAuthアプリには、"**WindowsAzureActiveDirectoryIntegratedApp**" というタグがあります。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="5f5b5-110">Gallery SAML Appsには、"**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**" というタグがあります。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="5f5b5-111">非ギャラリー SAML アプリには、"**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**" というタグがあります。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="5f5b5-112">したがって、これらのタグを使用して、それがどのようなアプリであるかを調べることができます。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="5f5b5-113">タグ "**WindowsAzureActiveDirectoryIntegratedApp**" は、すべての種類のアプリに共通です。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="5f5b5-114">次のスニペットを使用して、すべての SAML アプリ (ギャラリーと非ギャラリーの両方) を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="5f5b5-115">詳細については、「[AzureAD で SAML 対応アプリを特定する](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="5f5b5-116">**Web アプリケーションのみを検索して一覧表示する**: 以下のコマンドを使用して、アプリケーション タイプが "Web app/API" のすべての AzureAD アプリケーションを取得します。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="5f5b5-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="5f5b5-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="5f5b5-118">**ネイティブ アプリケーションのみを検索して一覧表示する**: 次のコマンドを実行して、すべてのネイティブ クライアント (デスクトップ/モバイルデバイス) アプリケーションを取得します。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="5f5b5-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="5f5b5-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="5f5b5-120">**登録されているすべての AzureAD アプリケーションの詳細を CSV にエクスポートする**: 次のコマンドは、必要な詳細を含むすべての AzureAD アプリを csv ファイルにエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="5f5b5-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="5f5b5-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="5f5b5-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="5f5b5-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="5f5b5-123">**未使用の Azure アプリのリストをエクスポートする必要がある** – 監査レポート</span><span class="sxs-lookup"><span data-stu-id="5f5b5-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="5f5b5-124">Azure AD Premium ライセンスを持っている場合、Azure AD は最大 30 日間のみアプリケーション ログを表示できます。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="5f5b5-125">30 日を超えてデータを保持するための 2 つのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="5f5b5-126">[Azure AD Reporting API](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) を使用して、プログラムでデータを取得し、データベースに保存できます。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="5f5b5-127">または、監査ログをサード パーティの SIEM システムに統合することもできます。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="5f5b5-128">[Azure ActiveDirectory] > [アプリ登録] > [ダウンロード] > [すべてのアプリケーション/所有アプリケーション] からすべてのアプリケーションと所有アプリケーションのアプリ リストをダウンロードすることもできます。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="5f5b5-129">MS Graph を介してアプリケーションのリストを取得するには、「[アプリケーションを一覧表示する - Microsoft Graphv1.0](https://docs.microsoft.com/graph/api/application-list)」および「[アプリケーション リソース タイプ - MicrosoftGraphv1.0](https://docs.microsoft.com/graph/api/resources/application)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f5b5-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>

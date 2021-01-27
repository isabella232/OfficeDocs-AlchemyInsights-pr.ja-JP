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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975115"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="e01ae-102">API を使用したアプリケーションの開発に関する問題</span><span class="sxs-lookup"><span data-stu-id="e01ae-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="e01ae-103">Azure Active Directory Graph API の使用を開始するには、「[Azure AD Graph API クイック スタート ガイド](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro)」を参照するか、「[対話型の Azure AD Graph API リファレンス ドキュメント](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)」を表示します。</span><span class="sxs-lookup"><span data-stu-id="e01ae-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="e01ae-104">**Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) のサポートの終了** _</span><span class="sxs-lookup"><span data-stu-id="e01ae-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="e01ae-105">**2020 年 6 月 30 日以降**、ADAL および Azure AD Graph に新しい機能は追加されなくなります。</span><span class="sxs-lookup"><span data-stu-id="e01ae-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="e01ae-106">テクニカル サポートおよびセキュリティ更新プログラムは引き続き提供されますが、機能の更新プログラムは提供されなくなります。</span><span class="sxs-lookup"><span data-stu-id="e01ae-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="e01ae-107">**2022 年 6月 30 日以降**、ADAL と Azure AD Graph のサポートは終了し、テクニカル サポートやセキュリティ更新プログラムは提供されなくなります。</span><span class="sxs-lookup"><span data-stu-id="e01ae-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="e01ae-108">既存の OS バージョンで ADAL を使用するアプリは、この期間以降も引き続き機能しますが、テクニカル サポートやセキュリティ更新プログラムは提供されません。</span><span class="sxs-lookup"><span data-stu-id="e01ae-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="e01ae-109">これ以降に Azure AD Graph を使用するアプリは、Azure AD Graph エンドポイントからの応答を受信しなくなる場合があります。</span><span class="sxs-lookup"><span data-stu-id="e01ae-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="e01ae-110">**ADAL 移行**</span><span class="sxs-lookup"><span data-stu-id="e01ae-110">**ADAL Migration**</span></span>

<span data-ttu-id="e01ae-111">最新の機能とセキュリティ更新プログラムを備えた[Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) に更新することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e01ae-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="e01ae-112">Microsoft アプリを使用している場合は、Microsoft がサポート終了期限までにアプリケーションを MSAL に移行していることを確認し、継続的に MSAL の強化されたセキュリティと機能を利用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="e01ae-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="e01ae-113">[ADAL の FAQ を確認します](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。</span><span class="sxs-lookup"><span data-stu-id="e01ae-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="e01ae-114">[プラットフォームごとにアプリを移行する方法について説明します](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。</span><span class="sxs-lookup"><span data-stu-id="e01ae-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="e01ae-115">どのアプリが ADAL を使用しているかを理解するためにサポートが必要な場合は、すべてのアプリのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e01ae-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="e01ae-116">Microsoft サポートでは、テナントにあるすべての Microsoft ADAL 以外のアプリのリストも提供できます。</span><span class="sxs-lookup"><span data-stu-id="e01ae-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="e01ae-117">**AAD Graph の移行**</span><span class="sxs-lookup"><span data-stu-id="e01ae-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="e01ae-118">Azure AD Graph を使用しているアプリケーションの場合は、ガイダンスに従って [Azure AD Graph アプリを Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true) に移行してください。</span><span class="sxs-lookup"><span data-stu-id="e01ae-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="e01ae-119">[移行のチェックリストは、開始ポイントを提供します](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。</span><span class="sxs-lookup"><span data-stu-id="e01ae-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="e01ae-120">Azure アプリの登録ポータルには、AAD Graph を使用しているアプリケーションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="e01ae-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="e01ae-121">アプリのすべてのソース コードを確認し、該当する場合は、ISV またはアプリ プロバイダーに連絡することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e01ae-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="e01ae-122">Microsoft のサポートでは、テナントでのすべての AAD Graph の使用状況のリストを提供することもできます。</span><span class="sxs-lookup"><span data-stu-id="e01ae-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="e01ae-123">アプリから Microsoft Graph のデータにアクセスする場合、ユーザーまたは管理者は、同意のプロセスを通してそのアプリに正しいアクセス許可を付与する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e01ae-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="e01ae-124">[Microsoft Graph のアクセス許可リファレンス](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true)では、Microsoft Graph API の各主要なセットに関連付けられているアクセス許可について説明します。</span><span class="sxs-lookup"><span data-stu-id="e01ae-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="e01ae-125">また、アクセス許可の使用方法に関するガイダンスを提供しています。</span><span class="sxs-lookup"><span data-stu-id="e01ae-125">It also provides guidance about how to use the permissions.</span></span>

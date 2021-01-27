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
# <a name="issues-developing-applications"></a><span data-ttu-id="c1f8f-102">アプリケーションの開発に関する問題</span><span class="sxs-lookup"><span data-stu-id="c1f8f-102">Issues developing applications</span></span>

<span data-ttu-id="c1f8f-103">Azure Active Directory (AD) アプリを作成するときに発生する最も一般的な問題のトラブルシューティングを行うには、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="c1f8f-104">Chrome ブラウザーのみを使用してアプリケーションにサインインする際に問題が発生します</span><span class="sxs-lookup"><span data-stu-id="c1f8f-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="c1f8f-105">アプリケーションのトークンの有効期間の既定値を変更する方法がわかりません</span><span class="sxs-lookup"><span data-stu-id="c1f8f-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="c1f8f-106">アプリケーションの同意の仕組みに混乱しています</span><span class="sxs-lookup"><span data-stu-id="c1f8f-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="c1f8f-107">アプリケーションにアクセス許可を付与する方法がわかりません</span><span class="sxs-lookup"><span data-stu-id="c1f8f-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="c1f8f-108">委任されたアクセス許可とアプリケーションのアクセス許可の違いがわかりません</span><span class="sxs-lookup"><span data-stu-id="c1f8f-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="c1f8f-109">\***Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) のサポートの終了** _</span><span class="sxs-lookup"><span data-stu-id="c1f8f-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="c1f8f-110">2020 年 6 月 30 日以降、Azure Active Directory 認証ライブラリ (ADAL) および Azure AD Graph API (AAD Graph) に新しい機能を追加しなくなります。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="c1f8f-111">テクニカル サポートおよびセキュリティ更新プログラムは引き続き提供されますが、機能の更新プログラムは提供されなくなります。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="c1f8f-112">2022 年 6月 30 日に ADAL および AAD Graph のサポートは終了し、以降はテクニカル サポートやセキュリティ更新プログラムは提供されなくなります。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="c1f8f-113">この条件の結果、次のような影響があります。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="c1f8f-114">既存の OS バージョンで ADAL を使用するアプリは、この期間以降も引き続き機能しますが、テクニカル サポートやセキュリティ更新プログラムは提供されません。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="c1f8f-115">これ以降に AAD Graph を使用するアプリは、AAD Graph エンドポイントからの応答を受信しなくなる場合があります</span><span class="sxs-lookup"><span data-stu-id="c1f8f-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="c1f8f-116">_ *ADAL 移行*\*</span><span class="sxs-lookup"><span data-stu-id="c1f8f-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="c1f8f-117">Microsoft アプリを使用している場合、最新の機能とセキュリティ更新プログラムを備えた Microsoft Authentication Library (MSAL) に更新することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="c1f8f-118">この推奨事項は、Microsoft がサポート終了期限までにアプリを MSAL に移行するプロセスを開始することに関連しています。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="c1f8f-119">Microsoft アプリを MSAL に移行すると、アプリが継続的に MSAL の強化されたセキュリティと機能を利用できます。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="c1f8f-120">ADAL の FAQ を読む</span><span class="sxs-lookup"><span data-stu-id="c1f8f-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="c1f8f-121">プラットフォームごとにアプリを移行する方法に関する詳細情報</span><span class="sxs-lookup"><span data-stu-id="c1f8f-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="c1f8f-122">どのアプリが ADAL を使用しているかを理解するためにサポートが必要な場合は、すべてのアプリのソース コードを確認し、該当する場合は、独立系ソフトウェア ベンダー (ISV) またはアプリ プロバイダーに連絡することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="c1f8f-123">Microsoft サポートでは、テナントにあるすべての Microsoft ADAL 以外のアプリのリストも提供できます。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="c1f8f-124">**AAD Graph の移行**</span><span class="sxs-lookup"><span data-stu-id="c1f8f-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="c1f8f-125">AAD Graph を使用しているアプリケーションの場合は、ガイダンスに従って AAD Graph アプリを Microsoft Graph に移行してください。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="c1f8f-126">[移行のチェックリストは、開始ポイントを提供します](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="c1f8f-127">Azure アプリの登録ポータルには、AAD Graph を使用しているアプリケーションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="c1f8f-128">アプリのすべてのソース コードを確認し、該当する場合は、独立系ソフトウェア ベンダー (ISV) またはアプリ プロバイダーに連絡することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="c1f8f-129">Microsoft のサポートでは、テナントでの AAD Graph の使用状況に関する情報を提供することもできます。</span><span class="sxs-lookup"><span data-stu-id="c1f8f-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>








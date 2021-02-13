---
title: AD FS を展開する
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177828"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="ad7a4-102">AD FS を展開する</span><span class="sxs-lookup"><span data-stu-id="ad7a4-102">Deploy AD FS</span></span>

<span data-ttu-id="ad7a4-103">Active Directory フェデレーション サービス (AD FS) の展開では、オンプレミス インフラストラクチャを使用して、Office 365 サービスのユーザーを認証します。</span><span class="sxs-lookup"><span data-stu-id="ad7a4-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="ad7a4-104">フェデレーション サインインを使用すると、ユーザーは、Azure Active Directory (Azure AD) と統合されている Office 365 サービスおよびサービスとしてのソフトウェア (SaaS) アプリケーションにサインインできます。</span><span class="sxs-lookup"><span data-stu-id="ad7a4-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="ad7a4-105">フェデレーション サインインは、AD FS を介してオンプレミスの Active Directory に対してユーザーを認証します。</span><span class="sxs-lookup"><span data-stu-id="ad7a4-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="ad7a4-106">また、企業ネットワーク上では、ユーザーはパスワードを再入力する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="ad7a4-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="ad7a4-107">[AD FS 展開アドバイザー](https://go.microsoft.com/fwlink/?linkid=2071178)は、Microsoft 365 および Office 365 サービスのユーザーを認証するオンプレミス AD FS インフラストラクチャの展開に関する段階的なガイダンスを提供します。</span><span class="sxs-lookup"><span data-stu-id="ad7a4-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="ad7a4-108">このガイドを使用すると、組織は AD FS コンポーネントと要件を確認し、展開に必要な SSL 証明書を取得してインストールし、必要な Web アプリケーション プロキシ サーバーをインストールできます。</span><span class="sxs-lookup"><span data-stu-id="ad7a4-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>

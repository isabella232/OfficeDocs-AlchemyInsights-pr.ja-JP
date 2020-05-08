---
title: 既定の Yammer ドメインを変更する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 099feb5c58a2b1068a2ec501ff966c6ac73d804d
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/01/2020
ms.locfileid: "44012663"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a><span data-ttu-id="1dfd0-102">既定の、または主要な Yammer ドメインを変更する</span><span class="sxs-lookup"><span data-stu-id="1dfd0-102">Changing the default/primary Yammer domain</span></span>

<span data-ttu-id="1dfd0-103">Yammer の URL には、Yammer ネットワークの現在のプライマリ ドメイン名が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-103">The Yammer URL contains the current primary domain name for your Yammer network.</span></span> <span data-ttu-id="1dfd0-104">このドメイン名は、Office 365 または Azure AD で設定されているプライマリ ドメイン名と一致しない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-104">This domain name may not match the primary domain name set in Office 365 or Azure AD.</span></span> <span data-ttu-id="1dfd0-105">テナントに追加されたカスタム ドメインの数や、Yammer がサポートされている構成 (1 テナント : 1 ネットワーク、または 1 : 1) に基づいて、動作に違いがあります。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-105">There are differences in behavior based on the number of custom domains added to the tenant, and whether Yammer is in a supported configuration (1 Tenant: 1 Network, or 1:1).</span></span> <span data-ttu-id="1dfd0-106">[Yammer ドメインおよび Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) の説明書については、こちらを参照してください。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-106">Documentation on [Yammer domains and Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) is available.</span></span>

<span data-ttu-id="1dfd0-107">間違ったドメインが表示される最も一般的な理由は、複数の Yammer ネットワークが存在し、統合する必要があることです。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-107">The most common reason that you see an incorrect domain is that multiple Yammer networks exist and need to be consolidated.</span></span> <span data-ttu-id="1dfd0-108">ネットワーク移行ツールを使用して[1つのネットワークに統合](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)することは、重要な第一歩です。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-108">[Consolidating down to a single network](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) using the network migration tool is an important first step.</span></span> <span data-ttu-id="1dfd0-109">プライマリ ドメインを設定する前にこれを完了します。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-109">Complete this before attempting to set your primary domain.</span></span>

<span data-ttu-id="1dfd0-110">**カスタム ドメインはありません**</span><span class="sxs-lookup"><span data-stu-id="1dfd0-110">**No custom domains**</span></span>

<span data-ttu-id="1dfd0-111">新しいテナントの場合、テナントからの既定のドメイン (たとえば、fabrikam.onmicrosoft.com) が Yammer に使用されます。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-111">For new tenants, the default domain (e.g. fabrikam.onmicrosoft.com) from the tenant will be used for Yammer.</span></span> <span data-ttu-id="1dfd0-112">プライマリ ドメインが yammer.com / fabrikam.onmicrosoft.com に設定されます。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-112">The primary domain is set to yammer.com/fabrikam.onmicrosoft.com.</span></span>

<span data-ttu-id="1dfd0-113">**単一のカスタムドメイン**</span><span class="sxs-lookup"><span data-stu-id="1dfd0-113">**Single custom domain**</span></span>

<span data-ttu-id="1dfd0-114">Yammer では、カスタム ドメイン (fabrikam.com など) が Yammer のプライマリ ドメインとしてテナントから自動的に選択されます。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-114">Yammer will automatically select the custom domain (e.g. fabrikam.com) from the tenant as the primary domain in Yammer.</span></span> <span data-ttu-id="1dfd0-115">Yammer.com / fabrikam.com に設定されます。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-115">It is set to yammer.com/fabrikam.com.</span></span> <span data-ttu-id="1dfd0-116">この変更は、ドメイン同期サービスによって実行され、最大で24時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-116">This change is made by the domain sync service, and can take up to 24 hours to take effect.</span></span>

<span data-ttu-id="1dfd0-117">**複数のカスタムドメイン**</span><span class="sxs-lookup"><span data-stu-id="1dfd0-117">**Multiple custom domains**</span></span>

<span data-ttu-id="1dfd0-118">Yammer は、既定のテナント ドメインとは異なるプライマリ ドメインを持つことができます。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-118">Yammer can have a primary domain that is different from the default tenant domain.</span></span> <span data-ttu-id="1dfd0-119">複数のカスタム ドメインがあるので、Yammer では、使用可能なドメインから正しいドメインを推測しません。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-119">Since there are multiple custom domains, Yammer does not attempt to guess the correct domain from those available.</span></span> <span data-ttu-id="1dfd0-120">プライマリドメイン名が選択したプライマリドメインに変更されるようにするには、サポート案件を依頼する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-120">You need to open a support case to request that the primary domain name is changed to the primary domain of your choice.</span></span>

<span data-ttu-id="1dfd0-121">**その他のトラブルシューティング情報**</span><span class="sxs-lookup"><span data-stu-id="1dfd0-121">**Additional troubleshooting information**</span></span>

<span data-ttu-id="1dfd0-122">場合によっては、ドメインがテナント間で移動されていて、ドメイン同期サービスが正常に実行されていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-122">In some cases domains may have been moved between tenants and the domain sync service has not been able to run successfully.</span></span> <span data-ttu-id="1dfd0-123">サインインまたはその他の問題に加えて、プライマリドメインが正しくない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-123">You may experience sign-in or other issues, in addition to an incorrect primary domain.</span></span> <span data-ttu-id="1dfd0-124">この問題を解決するには、Microsoft サポートによる支援を受け、ドメインを正しいネットワークに移動する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-124">To resolve this problem, domains may need to be moved to the correct network with help from Microsoft Support.</span></span> <span data-ttu-id="1dfd0-125">特に、ドメイン名のリストが非常に長い場合、このような状況は直接的な支援と解決に時間がかかる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-125">This situation requires direct assistance and can take some time to resolve, especially if there is a very long list of domain names.</span></span> <span data-ttu-id="1dfd0-126">サポート案件を開いて、これらの種類の問題の解決方法をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-126">Open a support case to get assistance with resolving these types of issues.</span></span>

<span data-ttu-id="1dfd0-127">サポートエージェントを使用している場合は、管理者が管理しているテナントでドメインが検証されます。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-127">When working with a support agent, they will check that domains are verified on a tenant under your control.</span></span> <span data-ttu-id="1dfd0-128">ユーザーがテナントに追加されても、DNS によって確認されない場合は、ドメインに関する追加認証の質問を求められることがあります。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-128">They may ask additional verification questions about your domains if they are added to your tenant but not verified by DNS.</span></span> <span data-ttu-id="1dfd0-129">ドメインが DNS によって確認され、プロセスが高速化されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="1dfd0-129">Please ensure that domains are verified by DNS to speed up the process.</span></span>

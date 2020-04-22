---
title: セットアップ DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645677"
---
# <a name="setup-dkim"></a><span data-ttu-id="a14c8-102">セットアップ DKIM</span><span class="sxs-lookup"><span data-stu-id="a14c8-102">Setup DKIM</span></span>

<span data-ttu-id="a14c8-103">Microsoft 365 でカスタムドメイン用に DKIM を構成する手順の詳細については、[以下](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a14c8-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="a14c8-104">カスタム ドメイン**ごと**に、ドメインの DNS ホスティング サービス (通常はドメイン レジストラー) で **2 つ**の DKIM CNAME レコードを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a14c8-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="a14c8-105">たとえば、contoso.com と fourthcoffee.com には、4 つの DKIM CNAME レコード (contoso.com と fourthcoffee.com のそれぞれに 2 つずつ) が必要になります。</span><span class="sxs-lookup"><span data-stu-id="a14c8-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="a14c8-106">**それぞれ**のカスタム ドメインの DKIM CNAME レコードには、次の書式を使用します。</span><span class="sxs-lookup"><span data-stu-id="a14c8-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="a14c8-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="a14c8-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="a14c8-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="a14c8-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="a14c8-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="a14c8-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="a14c8-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="a14c8-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="a14c8-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="a14c8-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="a14c8-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="a14c8-112">**TTL**: 3600</span></span>

   <span data-ttu-id="a14c8-113">\<DomainGUID\> は、カスタム ドメイン用にカスタマイズした MX レコードの `.mail.protection.outlook.com` の左側のテキストです (たとえば、ドメイン contoso.com の場合は `contoso-com` になります)。</span><span class="sxs-lookup"><span data-stu-id="a14c8-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="a14c8-114">\<InitialDomain\>は、Microsoft 365 へのサインアップ時に使用したドメインです (たとえば、contoso.onmicrosoft.com)。</span><span class="sxs-lookup"><span data-stu-id="a14c8-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="a14c8-115">カスタム ドメインの CNAME レコードを作成したら、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="a14c8-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="a14c8-116">a. </span><span class="sxs-lookup"><span data-stu-id="a14c8-116">a.</span></span> <span data-ttu-id="a14c8-117">[Microsoft 365 に](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)職場または学校のアカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="a14c8-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="a14c8-118">b. </span><span class="sxs-lookup"><span data-stu-id="a14c8-118">b.</span></span> <span data-ttu-id="a14c8-119">左上にあるアプリ起動ツールのアイコンを選択して、**[管理]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a14c8-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="a14c8-120">c. </span><span class="sxs-lookup"><span data-stu-id="a14c8-120">c.</span></span> <span data-ttu-id="a14c8-121">左下のナビゲーションで、**[管理者]** を展開し、**[Exchange]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a14c8-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="a14c8-122">d. </span><span class="sxs-lookup"><span data-stu-id="a14c8-122">d.</span></span> <span data-ttu-id="a14c8-123">**[保護]** > **[DKIM]** に移動します。</span><span class="sxs-lookup"><span data-stu-id="a14c8-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="a14c8-124">e. </span><span class="sxs-lookup"><span data-stu-id="a14c8-124">e.</span></span> <span data-ttu-id="a14c8-125">ドメインを選択してから、**[このドメインのメッセージに DKIM 署名を追加します]** に **[有効]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a14c8-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="a14c8-126">カスタム ドメインごとに、この手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="a14c8-126">Repeat this step for each custom domain.</span></span>

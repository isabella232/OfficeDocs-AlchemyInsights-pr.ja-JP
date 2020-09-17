---
title: DKIM のセットアップ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808712"
---
# <a name="setup-dkim"></a><span data-ttu-id="08d9b-102">DKIM のセットアップ</span><span class="sxs-lookup"><span data-stu-id="08d9b-102">Setup DKIM</span></span>

<span data-ttu-id="08d9b-103">Microsoft 365 のカスタム ドメイン用に DKIM を構成するための詳細な手順については、[こちら](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08d9b-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="08d9b-104">カスタム ドメイン**ごと**に、ドメインの DNS ホスティング サービス (通常はドメイン レジストラー) で **2 つ**の DKIM CNAME レコードを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="08d9b-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="08d9b-105">たとえば、contoso.com と fourthcoffee.com には、4 つの DKIM CNAME レコード (contoso.com と fourthcoffee.com のそれぞれに 2 つずつ) が必要になります。</span><span class="sxs-lookup"><span data-stu-id="08d9b-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="08d9b-106">**それぞれ**のカスタム ドメインの DKIM CNAME レコードには、次の書式を使用します。</span><span class="sxs-lookup"><span data-stu-id="08d9b-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="08d9b-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="08d9b-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="08d9b-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="08d9b-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="08d9b-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="08d9b-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="08d9b-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="08d9b-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="08d9b-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="08d9b-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="08d9b-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="08d9b-112">**TTL**: 3600</span></span>

   <span data-ttu-id="08d9b-113">\<DomainGUID\> は、カスタム ドメイン用にカスタマイズした MX レコードの `.mail.protection.outlook.com` の左側のテキストです (たとえば、ドメイン contoso.com の場合は `contoso-com` になります)。</span><span class="sxs-lookup"><span data-stu-id="08d9b-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="08d9b-114">\<InitialDomain\> は、Microsoft 365 のサインアップ時に使用したドメインです (たとえば、contoso.onmicrosoft.com)。</span><span class="sxs-lookup"><span data-stu-id="08d9b-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="08d9b-115">カスタム ドメインの CNAME レコードを作成したら、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="08d9b-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="08d9b-116">a. </span><span class="sxs-lookup"><span data-stu-id="08d9b-116">a.</span></span> <span data-ttu-id="08d9b-117">職場または学校アカウントを使用して、[Microsoft 365 にサインイン](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)します。</span><span class="sxs-lookup"><span data-stu-id="08d9b-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="08d9b-118">b. </span><span class="sxs-lookup"><span data-stu-id="08d9b-118">b.</span></span> <span data-ttu-id="08d9b-119">左上にあるアプリ起動ツールのアイコンを選択して、**[管理]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="08d9b-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="08d9b-120">c. </span><span class="sxs-lookup"><span data-stu-id="08d9b-120">c.</span></span> <span data-ttu-id="08d9b-121">左下のナビゲーションで、**[管理者]** を展開し、**[Exchange]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="08d9b-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="08d9b-122">d. </span><span class="sxs-lookup"><span data-stu-id="08d9b-122">d.</span></span> <span data-ttu-id="08d9b-123">**[保護]** > **[DKIM]** に移動します。</span><span class="sxs-lookup"><span data-stu-id="08d9b-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="08d9b-124">e. </span><span class="sxs-lookup"><span data-stu-id="08d9b-124">e.</span></span> <span data-ttu-id="08d9b-125">ドメインを選択してから、**[このドメインのメッセージに DKIM 署名を追加します]** に **[有効]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="08d9b-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="08d9b-126">カスタム ドメインごとに、この手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="08d9b-126">Repeat this step for each custom domain.</span></span>

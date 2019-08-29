---
title: Office 365 の DKIM をセットアップする
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666269"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="b5c4c-102">Office 365 の DKIM をセットアップする</span><span class="sxs-lookup"><span data-stu-id="b5c4c-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="b5c4c-103">Office 365 のカスタム ドメイン用に DKIM を構成するための手順については、[ここ](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5c4c-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="b5c4c-104">カスタム ドメイン**ごと**に、ドメインの DNS ホスティング サービス (通常はドメイン レジストラー) で **2 つ**の DKIM CNAME レコードを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b5c4c-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="b5c4c-105">たとえば、contoso.com と fourthcoffee.com には、4 つの DKIM CNAME レコード (contoso.com と fourthcoffee.com のそれぞれに 2 つずつ) が必要になります。</span><span class="sxs-lookup"><span data-stu-id="b5c4c-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="b5c4c-106">**それぞれ**のカスタム ドメインの DKIM CNAME レコードには、次の書式を使用します。</span><span class="sxs-lookup"><span data-stu-id="b5c4c-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="b5c4c-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="b5c4c-107">**Host name**</span></span>

     <span data-ttu-id="b5c4c-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="b5c4c-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="b5c4c-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="b5c4c-109">TTL: 3600</span></span>

   - <span data-ttu-id="b5c4c-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="b5c4c-110">**Host name**</span></span>

     <span data-ttu-id="b5c4c-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="b5c4c-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="b5c4c-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="b5c4c-112">TTL: 3600</span></span>

   <span data-ttu-id="b5c4c-113">\<DomainGUID\> は、カスタム ドメイン用にカスタマイズした MX レコードの `.mail.protection.outlook.com` の左側のテキストです (たとえば、ドメイン contoso.com の場合は `contoso-com` になります)。</span><span class="sxs-lookup"><span data-stu-id="b5c4c-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="b5c4c-114">\<InitialDomain\> は、Office 365 のサインアップ時に使用したドメインです (たとえば、contoso.onmicrosoft.com)。</span><span class="sxs-lookup"><span data-stu-id="b5c4c-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="b5c4c-115">カスタム ドメインの CNAME レコードを作成したら、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="b5c4c-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="b5c4c-116">a. </span><span class="sxs-lookup"><span data-stu-id="b5c4c-116">a.</span></span> <span data-ttu-id="b5c4c-117">職場または学校のアカウントを使用して、[Office 365 にサインイン](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)します。</span><span class="sxs-lookup"><span data-stu-id="b5c4c-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="b5c4c-118">b. </span><span class="sxs-lookup"><span data-stu-id="b5c4c-118">b.</span></span> <span data-ttu-id="b5c4c-119">左上にあるアプリ起動ツールのアイコンを選択して、**[管理]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b5c4c-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="b5c4c-120">c. </span><span class="sxs-lookup"><span data-stu-id="b5c4c-120">c.</span></span> <span data-ttu-id="b5c4c-121">左下のナビゲーションで、**[管理者]** を展開し、**[Exchange]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b5c4c-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="b5c4c-122">d. </span><span class="sxs-lookup"><span data-stu-id="b5c4c-122">d.</span></span> <span data-ttu-id="b5c4c-123">**[保護]** > **[DKIM]** に移動します。</span><span class="sxs-lookup"><span data-stu-id="b5c4c-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="b5c4c-124">e. </span><span class="sxs-lookup"><span data-stu-id="b5c4c-124">e.</span></span> <span data-ttu-id="b5c4c-125">ドメインを選択してから、**[このドメインのメッセージに DKIM 署名を追加します]** に **[有効]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b5c4c-125">Select the domain for which you want to enable DKIM and then, for **Sign messages for this domain with DKIM signatures**, choose **Enable**.</span></span> <span data-ttu-id="b5c4c-126">カスタム ドメインごとに、この手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="b5c4c-126">Repeat this step for each custom domain.</span></span>

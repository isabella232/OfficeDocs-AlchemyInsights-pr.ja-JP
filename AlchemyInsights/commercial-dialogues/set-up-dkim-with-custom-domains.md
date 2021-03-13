---
title: カスタム ドメインを使用して DKIM をセットアップする
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751189"
---
# <a name="set-up-dkim-with-custom-domains"></a><span data-ttu-id="f14b4-102">カスタム ドメインを使用して DKIM をセットアップする</span><span class="sxs-lookup"><span data-stu-id="f14b4-102">Set up DKIM with custom domains</span></span>

<span data-ttu-id="f14b4-103">DNS で各カスタム ドメインに対して 2 つの CNAME レコードを発行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f14b4-103">You must publish two CNAME records for each custom domain in DNS.</span></span> <span data-ttu-id="f14b4-104">そのためには、次の形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="f14b4-104">To do this, use the following format:</span></span>

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> <span data-ttu-id="f14b4-105">**DomainGUID** は、カスタム ドメインのカスタマイズされた MX レコード (たとえば、ドメイン **contoso.com** の contoso-com) の **.mail.protection.outlook.com** の左側にあるテキストです。</span><span class="sxs-lookup"><span data-stu-id="f14b4-105">**DomainGUID** is the text to the left of **.mail.protection.outlook.com** in the customized MX record for the custom domain (for example, contoso-com for the domain **contoso.com**).</span></span> <span data-ttu-id="f14b4-106">**InitialDomain** は、Office 365 のサインアップ時に使用したドメインです (たとえば、**contoso.onmicrosoft.com**)。</span><span class="sxs-lookup"><span data-stu-id="f14b4-106">**InitialDomain** is the domain you used when you signed up for Office 365 (for example, **contoso.onmicrosoft.com**).</span></span>

<span data-ttu-id="f14b4-107">DNS に関する詳細については、「[任意の DNS ホスティング プロバイダーで Office 365 用に DNS レコードを作成する](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f14b4-107">For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>
---
title: Microsoft で購入または管理されているドメインで Wix Web サイトを使用する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: f6845c56f05e9cef11362ce601a974b73a154c9a
ms.sourcegitcommit: 28a319e482e6a8644e87726e1b0e599819df52d0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2020
ms.locfileid: "46630060"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a><span data-ttu-id="82b5a-102">Microsoft で購入または管理されているドメインで Wix Web サイトを使用する</span><span class="sxs-lookup"><span data-stu-id="82b5a-102">Using a Wix website with Microsoft purchased or managed domains</span></span>

<span data-ttu-id="82b5a-103">Microsoft で購入または管理されているドメインで Wix Web サイトを使用する方法の詳細については、「[DNS レコードを更新して現在のホスティング プロバイダーに Web サイトを維持する](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82b5a-103">For information about how to use a Wix website with a Microsoft purchased or managed domain, see [Update DNS records to keep your website with your current hosting provider](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span></span>

<span data-ttu-id="82b5a-104">詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82b5a-104">For details, see:</span></span> 

- <span data-ttu-id="82b5a-105">Wix の記事「ポインティング方式を使用した Wix にドメインを接続する」では、Microsoft 365 を使用するときにネーム サーバーを変更するのではなく、上記のリンクに従って DNS レコードを追加することを推奨しています。</span><span class="sxs-lookup"><span data-stu-id="82b5a-105">The Wix article, "Connecting a Domain to Wix Using the Pointing Method," recommends adding DNS records as outlined in the link above rather than changing names servers when you're using Microsoft 365.</span></span>

- <span data-ttu-id="82b5a-106">それでもネーム サーバーを Wix に変更する場合は、Microsoft 用 Wix で DNS レコードを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="82b5a-106">If you choose to change name servers to Wix, you must create DNS records at Wix for Microsoft.</span></span> <span data-ttu-id="82b5a-107">詳細については、「[Microsoft 用 Wix で DNS レコードを作成する](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82b5a-107">For more info, see [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span></span>

- <span data-ttu-id="82b5a-108">ドメインを Microsoft から購入した場合、ネーム サーバーは変更できません。</span><span class="sxs-lookup"><span data-stu-id="82b5a-108">If your domain was purchased from Microsoft the name servers can't be changed.</span></span> <span data-ttu-id="82b5a-109">ネーム サーバーを変更する必要がある場合は、Microsoft が購入したドメインを 60 日後に別のホスティング プロバイダーに移管する必要があります。</span><span class="sxs-lookup"><span data-stu-id="82b5a-109">If you must change names servers, the Microsoft purchased domain must be transferred to another hosting provider after 60 days.</span></span> <span data-ttu-id="82b5a-110">詳細については、「[ドメインに関する FAQ](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82b5a-110">For more info, see the [Domains FAQ](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span></span>
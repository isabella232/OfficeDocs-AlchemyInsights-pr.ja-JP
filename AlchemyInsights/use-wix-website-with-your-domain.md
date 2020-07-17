---
title: Office 365 で購入または管理されているドメインで Wix Web サイトを使用する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 64dfe6082bea1e468eae78bf1576fde398e4c28a
ms.sourcegitcommit: 3ca312535d950105ee829e037f0ff8f1ddbbae72
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2020
ms.locfileid: "44708605"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a><span data-ttu-id="d8a68-102">Office 365 で購入または管理されているドメインで Wix Web サイトを使用する</span><span class="sxs-lookup"><span data-stu-id="d8a68-102">Using Wix website with Office 365 purchased or managed domains</span></span>

- [<span data-ttu-id="d8a68-103">DNS レコードを更新して現在のホスティング プロバイダーに Web サイトを維持する</span><span class="sxs-lookup"><span data-stu-id="d8a68-103">Update DNS records to keep your website with your current hosting provider</span></span>](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- <span data-ttu-id="d8a68-104">Wix の記事「ポインティング方式を使用した Wix にドメインを接続する」では、Office 365 を使用するときにネーム サーバーを変更するのではなく、ポインティング (上記のリンクに従って DNS レコードを追加) を使用することを推奨しています</span><span class="sxs-lookup"><span data-stu-id="d8a68-104">Wix article "Connecting a Domain to Wix Using the Pointing Method" recommends using pointing (adding DNS records per the above link) rather than changing names servers when using Office 365</span></span>
- <span data-ttu-id="d8a68-105">それでもネーム サーバーを Wix に変更する場合は、[Microsoft の Wix で DNS レコードを作成する](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8a68-105">If you still choose to change name servers to Wix you will then need to  [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)</span></span>
- <span data-ttu-id="d8a68-106">ドメインを Microsoft から購入した場合、ネーム サーバーは変更できません。</span><span class="sxs-lookup"><span data-stu-id="d8a68-106">If your domain was purchased from Microsoft the name servers cannot be changed.</span></span> <span data-ttu-id="d8a68-107">ネーム サーバーを変更する必要がある場合は、Microsoft が購入したドメインを [60 日後に別のホスティング プロバイダーに移管する必要があります](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)</span><span class="sxs-lookup"><span data-stu-id="d8a68-107">If you have to change names servers the Microsoft purchased domain would need to be  [transferred to another hosting provider after 60 days](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)</span></span>
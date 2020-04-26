---
title: ドメインの転送
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002570"
- "4985"
ms.openlocfilehash: 4508c70331f8d83f9f3569c64d49e963af801eb9
ms.sourcegitcommit: 6ecb6fcbd738b8896c5d616130074438a1a6e357
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2020
ms.locfileid: "43543513"
---
# <a name="domain-transfers"></a><span data-ttu-id="12eaf-102">ドメインの転送</span><span class="sxs-lookup"><span data-stu-id="12eaf-102">Domain transfers</span></span>

- <span data-ttu-id="12eaf-103">[Microsoft が購入したドメインを60日後に別のプロバイダーに移行する方法](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq?view=o365-worldwide#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)。</span><span class="sxs-lookup"><span data-stu-id="12eaf-103">[How to transfer a Microsoft purchased domain to another provider after 60 days](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq?view=o365-worldwide#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span></span>

    - <span data-ttu-id="12eaf-104">Microsoft が購入したドメインでは NS レコードの変更はサポートされていませんが、Web ホスティングにドメイン登録を転送するのではなく、[Web サイトの DNS レコードの更新をする](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider?view=o365-worldwide)ことを検討してください。</span><span class="sxs-lookup"><span data-stu-id="12eaf-104">Although Microsoft purchased domains don't support changing NS records, consider [updating DNS records for your website](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider?view=o365-worldwide) instead of transferring your domain registration to the web hoster.</span></span>

- <span data-ttu-id="12eaf-105">Microsoft が購入したドメインは、Office 365 テナント間で転送することはできません。</span><span class="sxs-lookup"><span data-stu-id="12eaf-105">A Microsoft purchased domain cannot be transferred between Office 365 tenants.</span></span> 

    - <span data-ttu-id="12eaf-106">ただし、[1つのテナントからドメインを削除](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain?view=o365-worldwide)してから、別のテナントのドメインを確認することによって、Office 365 テナント間でサードパーティのドメインを転送できます。</span><span class="sxs-lookup"><span data-stu-id="12eaf-106">However, you can transfer a third-party domain between Office 365 tenants by [removing the domain from one tenant](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain?view=o365-worldwide) and then verifying the domain in another tenant.</span></span>

- <span data-ttu-id="12eaf-107">サードパーティのドメイン登録や課金は、Microsoft に転送できません。</span><span class="sxs-lookup"><span data-stu-id="12eaf-107">A third-party domains registration or billing cannot be transferred to Microsoft.</span></span>

    - <span data-ttu-id="12eaf-108">ただし、カスタムドメインを [検証し、Microsoft 365で使用することができます](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="12eaf-108">But custom domains can be  [verified and used with Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain?view=o365-worldwide).</span></span>

- <span data-ttu-id="12eaf-109">Onmicrosoft.com の初期デフォルトドメインの転送や名前の変更はできません。</span><span class="sxs-lookup"><span data-stu-id="12eaf-109">Onmicrosoft.com initial default domains cannot be transferred or renamed.</span></span>

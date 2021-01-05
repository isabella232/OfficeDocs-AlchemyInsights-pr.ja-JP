---
title: テナント間でドメインを転送する
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/2/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002570"
- "7305"
ms.openlocfilehash: d696c9d095fb6b2b374d8c5872e94cc7e32dceb8
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/02/2020
ms.locfileid: "49565249"
---
# <a name="transfer-domain-between-tenants"></a><span data-ttu-id="0aca1-102">テナント間でドメインを転送する</span><span class="sxs-lookup"><span data-stu-id="0aca1-102">Transfer domain between tenants</span></span>

<span data-ttu-id="0aca1-103">forthcoffee.com のようなカスタム ドメインは、あるテナントから手動で削除し、その後新しいテナントで検証することができます。</span><span class="sxs-lookup"><span data-stu-id="0aca1-103">A custom domain such as forthcoffee.com can be manually removed from one tenant and then verified in a new tenant.</span></span>

<span data-ttu-id="0aca1-104">次の手順で[ドメインを削除](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain)します。</span><span class="sxs-lookup"><span data-stu-id="0aca1-104">Follow these steps to [Remove a domain](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain).</span></span> <span data-ttu-id="0aca1-105">次に、新しいテナントで、**[設定]** > **[ドメイン]** > **[ドメインの追加]** の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="0aca1-105">Then in the new tenant go to **Settings** > **Domains** > **Add domain**.</span></span>

<span data-ttu-id="0aca1-106">より複雑なシナリオについては、「[Microsoft 365 tenant-to-tenant migrations (Microsoft 365 のテナントからテナントへの移行)](https://docs.microsoft.com/microsoft-365/enterprise/microsoft-365-tenant-to-tenant-migrations)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0aca1-106">For more complex scenarios, see [Microsoft 365 tenant-to-tenant migrations](https://docs.microsoft.com/microsoft-365/enterprise/microsoft-365-tenant-to-tenant-migrations).</span></span>

<span data-ttu-id="0aca1-107">**以下の点にもご注意ください**。</span><span class="sxs-lookup"><span data-stu-id="0aca1-107">**Also note**:</span></span>
- <span data-ttu-id="0aca1-108">初期ドメインの onmicrosoft.com を削除したり、テナント間で移動したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="0aca1-108">The initial onmicrosoft.com domain cannot be deleted or moved between tenants.</span></span>
- <span data-ttu-id="0aca1-109">Microsoft から購入したカスタム ドメインをテナント間で移動することはできません。</span><span class="sxs-lookup"><span data-stu-id="0aca1-109">A custom domain purchased from Microsoft cannot be moved between tenants.</span></span>
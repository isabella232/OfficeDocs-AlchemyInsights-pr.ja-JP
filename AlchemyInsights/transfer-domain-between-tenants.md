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
ms.openlocfilehash: 942ca306951fdd8e971ea27da88af5601325185b7c169b4df3dfd9e43e1650c5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048629"
---
# <a name="transfer-domain-between-tenants"></a>テナント間でドメインを転送する

forthcoffee.com のようなカスタム ドメインは、あるテナントから手動で削除し、その後新しいテナントで検証することができます。

次の手順で[ドメインを削除](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain)します。 次に、新しいテナントで、**[設定]** > **[ドメイン]** > **[ドメインの追加]** の順に移動します。

より複雑なシナリオについては、「[Microsoft 365 tenant-to-tenant migrations (Microsoft 365 のテナントからテナントへの移行)](https://docs.microsoft.com/microsoft-365/enterprise/microsoft-365-tenant-to-tenant-migrations)」を参照してください。

**以下の点にもご注意ください**。
- 初期ドメインの onmicrosoft.com を削除したり、テナント間で移動したりすることはできません。
- Microsoft から購入したカスタム ドメインをテナント間で移動することはできません。
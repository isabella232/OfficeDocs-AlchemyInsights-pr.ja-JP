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
ms.openlocfilehash: e78b560329254f7035869c076db5ff31427dc7ae
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2020
ms.locfileid: "43783976"
---
# <a name="domain-transfers"></a>ドメインの転送

- [Microsoft が購入したドメインを60日後に別のプロバイダーに移行する方法](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq?view=o365-worldwide#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)。

    - Microsoft が購入したドメインでは NS レコードの変更はサポートされていませんが、Web ホスティングにドメイン登録を転送するのではなく、[Web サイトの DNS レコードの更新をする](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider?view=o365-worldwide)ことを検討してください。

- Microsoft が購入したドメインは、Microsoft 365 テナント間で転送することはできません。 

    - ただし、[1 つのテナントからドメインを削除](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain?view=o365-worldwide)してから、別のテナントのドメインを確認することによって、Microsoft 365 テナント間でサードパーティのドメインを転送できます。

- サードパーティのドメイン登録や課金は、Microsoft に転送できません。

    - ただし、カスタムドメインを [検証し、Microsoft 365で使用することができます](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain?view=o365-worldwide)。

- Onmicrosoft.com の初期デフォルトドメインの転送や名前の変更はできません。

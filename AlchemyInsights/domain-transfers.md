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
# <a name="domain-transfers"></a>ドメインの転送

- [Microsoft が購入したドメインを60日後に別のプロバイダーに移行する方法](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq?view=o365-worldwide#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)。

    - Microsoft が購入したドメインでは NS レコードの変更はサポートされていませんが、Web ホスティングにドメイン登録を転送するのではなく、[Web サイトの DNS レコードの更新をする](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider?view=o365-worldwide)ことを検討してください。

- Microsoft が購入したドメインは、Office 365 テナント間で転送することはできません。 

    - ただし、[1つのテナントからドメインを削除](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain?view=o365-worldwide)してから、別のテナントのドメインを確認することによって、Office 365 テナント間でサードパーティのドメインを転送できます。

- サードパーティのドメイン登録や課金は、Microsoft に転送できません。

    - ただし、カスタムドメインを [検証し、Microsoft 365で使用することができます](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain?view=o365-worldwide)。

- Onmicrosoft.com の初期デフォルトドメインの転送や名前の変更はできません。

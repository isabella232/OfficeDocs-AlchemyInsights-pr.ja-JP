---
title: Office 365 で購入または管理されているドメインで Wix Web サイトを使用する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825952"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Office 365 で購入または管理されているドメインで Wix Web サイトを使用する

- [DNS レコードを更新して現在のホスティング プロバイダーに Web サイトを維持する](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix の記事「ポインティング方式を使用した Wix にドメインを接続する」では、Office 365 を使用するときにネーム サーバーを変更するのではなく、ポインティング (上記のリンクに従って DNS レコードを追加) を使用することを推奨しています
- それでもネーム サーバーを Wix に変更する場合は、[Microsoft の Wix で DNS レコードを作成する](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)必要があります。
- ドメインを Microsoft から購入した場合、ネーム サーバーは変更できません。 ネーム サーバーを変更する必要がある場合は、Microsoft が購入したドメインを [60 日後に別のホスティング プロバイダーに移管する必要があります](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
---
title: Microsoft ネーム サーバーから独自の DNS レコードの管理に戻る
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506164"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Microsoft ネーム サーバーから独自の DNS レコードの管理に戻る

以前に NS レコードを Microsoft (ns1.bdm.microsoftonline.com) を指すように変更しましたが、今度は独自の DNS レコードを管理することにしました。

ドメイン レジストラーの Web サイトで、ネーム サーバーをレジストラーまたは以前の設定に戻します。 DNS が不明の場合は、ドメイン レジストラーのサポートにお問い合わせください。 注: ネーム サーバーの変更は、反映されるまで最大 48 時間かかります。 

1. Microsoft 365 管理ポータルで、**[設定]** > [**[ドメイン]**](https://admin.microsoft.com/Adminportal/Home#/Domains) の順に移動し、ドメインの横にあるチェックボックスを選択して、**[DNSの管理]** を選択します。 

2. ウィザードで **[独自の DNS レコードを追加]** を選択し、ウィザードを完了します。 これにより、DNS の管理方法が変更され、選択したサービスをサポートするために必要なカスタム DNS レコードを追加できるようになります。

または、ネーム サーバー レコードを Microsoft に変更し、Web サイトがある場合は、ネーム サーバーを元に戻す代わりに、Web サイトの DNS レコードを追加できます。 詳細情報については、「[DNS レコードを更新して現在のホスティング プロバイダーに Web サイトを維持する](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)」をご覧ください。



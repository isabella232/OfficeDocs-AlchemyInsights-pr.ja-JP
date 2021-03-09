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
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527806"
---
# <a name="set-up-dkim-with-custom-domains"></a>カスタム ドメインを使用して DKIM をセットアップする

DNS で各カスタム ドメインに対して 2 つの CNAME レコードを発行する必要があります。 そのためには、次の形式を使用します。

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** は、カスタム ドメインのカスタマイズされた MX レコード (たとえば、ドメイン **contoso.com** の contoso-com) の **.mail.protection.outlook.com** の左側にあるテキストです。 **InitialDomain** は、Office 365 のサインアップ時に使用したドメインです (たとえば、**contoso.onmicrosoft.com**)。

DNS に関する詳細については、「[任意の DNS ホスティング プロバイダーで Office 365 用に DNS レコードを作成する](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)」を参照してください。
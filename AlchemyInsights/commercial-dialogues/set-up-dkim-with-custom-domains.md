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
ms.openlocfilehash: bb19f0672a21ea8b99c433ad83db4d89536c9a1705245fd2a683471170ab51ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994823"
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
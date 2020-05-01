---
title: DKIM のセットアップ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645677"
---
# <a name="setup-dkim"></a>DKIM のセットアップ

Microsoft 365 のカスタム ドメイン用に DKIM を構成するための詳細な手順については、[こちら](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)を参照してください。

1. カスタム ドメイン**ごと**に、ドメインの DNS ホスティング サービス (通常はドメイン レジストラー) で **2 つ**の DKIM CNAME レコードを作成する必要があります。 たとえば、contoso.com と fourthcoffee.com には、4 つの DKIM CNAME レコード (contoso.com と fourthcoffee.com のそれぞれに 2 つずつ) が必要になります。

   **それぞれ**のカスタム ドメインの DKIM CNAME レコードには、次の書式を使用します。

   - **Host name**: `selector1._domainkey.<CustomDomain>`

     **Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Host name**: `selector2._domainkey.<CustomDomain>`

     **Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> は、カスタム ドメイン用にカスタマイズした MX レコードの `.mail.protection.outlook.com` の左側のテキストです (たとえば、ドメイン contoso.com の場合は `contoso-com` になります)。 \<InitialDomain\> は、Microsoft 365 のサインアップ時に使用したドメインです (たとえば、contoso.onmicrosoft.com)。

2. カスタム ドメインの CNAME レコードを作成したら、次の手順を実行します。

   a.  職場または学校アカウントを使用して、[Microsoft 365 にサインイン](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)します。

   b.  左上にあるアプリ起動ツールのアイコンを選択して、**[管理]** をクリックします。

   c.  左下のナビゲーションで、**[管理者]** を展開し、**[Exchange]** を選択します。

   d.  **[保護]** > **[DKIM]** に移動します。

   e.  ドメインを選択してから、**[このドメインのメッセージに DKIM 署名を追加します]** に **[有効]** を選択します。 カスタム ドメインごとに、この手順を繰り返します。

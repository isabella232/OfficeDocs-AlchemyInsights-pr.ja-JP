---
title: Office 365 の DKIM をセットアップする
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666269"
---
# <a name="setup-dkim-in-office-365"></a>Office 365 の DKIM をセットアップする

Office 365 のカスタム ドメイン用に DKIM を構成するための手順については、[ここ](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)を参照してください。

1. カスタム ドメイン**ごと**に、ドメインの DNS ホスティング サービス (通常はドメイン レジストラー) で **2 つ**の DKIM CNAME レコードを作成する必要があります。 たとえば、contoso.com と fourthcoffee.com には、4 つの DKIM CNAME レコード (contoso.com と fourthcoffee.com のそれぞれに 2 つずつ) が必要になります。

   **それぞれ**のカスタム ドメインの DKIM CNAME レコードには、次の書式を使用します。

   - **Host name**: `selector1._domainkey.<CustomDomain>`

     **Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Host name**: `selector2._domainkey.<CustomDomain>`

     **Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> は、カスタム ドメイン用にカスタマイズした MX レコードの `.mail.protection.outlook.com` の左側のテキストです (たとえば、ドメイン contoso.com の場合は `contoso-com` になります)。 \<InitialDomain\> は、Office 365 のサインアップ時に使用したドメインです (たとえば、contoso.onmicrosoft.com)。

2. カスタム ドメインの CNAME レコードを作成したら、次の手順を実行します。

   a.  職場または学校のアカウントを使用して、[Office 365 にサインイン](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)します。

   b.  左上にあるアプリ起動ツールのアイコンを選択して、**[管理]** をクリックします。

   c.  左下のナビゲーションで、**[管理者]** を展開し、**[Exchange]** を選択します。

   d.  **[保護]** > **[DKIM]** に移動します。

   e.  ドメインを選択してから、**[このドメインのメッセージに DKIM 署名を追加します]** に **[有効]** を選択します。 カスタム ドメインごとに、この手順を繰り返します。

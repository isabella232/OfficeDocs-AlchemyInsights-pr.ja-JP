---
title: 米国の銀行口座番号の DLP ルールが機能しない場合
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507339"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>米国の銀行口座番号に関する DLP の問題

**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。

**米国の銀行口座番号に関する DLP の問題**

Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.
  
たとえば、85% の信頼レベルで構成された**米国の銀行口座番号**では、以下の内容が評価されるため、ルールをトリガーするためにはこれらの内容が検出される必要があります。
  
- **[書式:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8 ～ 17 桁の数字

- **[パターン:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8 ～ 17 桁の連続する数字。

- **[チェックサム:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** いいえ、チェックサムはありません。

- **[定義:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP ポリシーは、抽出した約 300 文字が次の条件に該当することを検出した場合に、75% の確証を持ってそれがこの種類の機密情報であると特定します。

  - 正規表現 Regex_usa_bank_account_number がパターンに一致するコンテンツを検出した

  - Keyword_usa_Bank_Account のキーワードを検出した。

    たとえば、次の当座預金口座 78344011 では、**米国の銀行口座番号** のポリシーがトリガーされます。

コンテンツに対して**米国の銀行口座番号**が検出されるために必要な情報の詳細については、この記事の「[米国の銀行口座番号 SSN に関する機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)」を参照してください。
  
さまざまな組み込みの機密情報の種類を使用している場合は、「[機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)」の記事でその他の種類に必要なものを参照してください。
  
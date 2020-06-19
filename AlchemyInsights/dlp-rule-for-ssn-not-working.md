---
title: SSN に関する DLP ルールが機能しない
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507375"
---
# <a name="dlp-issues-with-social-security-numbers"></a>社会保障番号に伴う DLP の問題

**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。

**SSN に関する DLP の問題**

Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365? If so, make sure your content contains the needed information for what the DLP policy is looking. 
  
たとえば、85% の信頼レベルで構成された SSN ポリシーでは、以下の内容が評価されるため、ルールをトリガーするためにはこれらの内容が検出される必要があります。
  
- **[書式:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 桁の数字、書式設定されたパターンの場合もあれば、書式設定されていないパターンの場合もあります。

- **[パターン:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 次の 4 つの関数が 4 つの異なるパターンで SSN を検索します。

  - Func_ssn は、2011 年以前の厳密な書式の SSN を検索します。これはダッシュまたはスペース (ddd-dd-dddd または ddd dd dddd) の形式になっています。

  - Func_unformatted_ssn は、2011 年以前の厳密な書式の SSN を検索します。これは 9 桁の連続した数字 (ddddddddd) の形式になっています。

  - Func_randomized_formatted_ssn は、2011 年以降の SSN を検索します。これはダッシュまたはスペース (ddd-dd-dddd または ddd dd dddd) の形式になっています。

  - Func_randomized_unformatted_ssn は、2011 年以降の SSN を検索します。これは 9 桁の連続した数字 (ddddddddd) の形式になっています。

- **[チェックサム:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** いいえ、チェックサムはありません。

- **[定義:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP ポリシーは、抽出した約 300 文字が次の条件に該当することを検出した場合に、85% の確証を持ってそれがこの種類の機密情報であると特定します。

  - [関数 Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) がパターンに一致するコンテンツを検出した。

  - A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found. Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  . For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**
  
コンテンツに対して SSN を検出するために必要なものに関する詳細については、この記事の「[SSN に関する機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)」を参照してください。
  
さまざまな組み込みの機密情報の種類を使用している場合は、「[機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)」の記事でその他の種類に必要なものを参照してください。
  
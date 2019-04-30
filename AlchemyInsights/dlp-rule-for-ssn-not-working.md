---
title: SSN に関する DLP ルールが機能しない
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 605f5e1a2f702998996246700f9f1d04a0bd0e9c
ms.sourcegitcommit: 6c104d686acbce8fa9adeaaedaa44b132b74321a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/29/2019
ms.locfileid: "33470093"
---
Office 365 で機密情報の類を使用しているときに、**社会保障番号 (SSN)** を含むコンテンツに対して**データ損失防止 (DLP)** が機能しないという問題は発生していませんか。発生している場合は、コンテンツに DLP ポリシーに必要な情報が含まれていることを確認してください。 
  
たとえば、85% の信頼レベルで構成された SSN ポリシーでは、以下の内容が評価されるため、ルールをトリガーするためにはこれらの内容が検出される必要があります。
  
- **[書式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 桁の数字、書式設定されたパターンの場合もあれば、書式設定されていないパターンの場合もあります。 
    
- **[パターン:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 次の 4 つの関数が 4 つの異なるパターンで SSN を検索します。 
    
  - Func_ssn は、2011 年以前の厳密な書式の SSN を検索します。これはダッシュまたはスペース (ddd-dd-dddd または ddd dd dddd) の形式になっています。
    
  - Func_unformatted_ssn は、2011 年以前の厳密な書式の SSN を検索します。これは 9 桁の連続した数字 (ddddddddd) の形式になっています。
    
  - Func_randomized_formatted_ssn は、2011 年以降の SSN を検索します。これはダッシュまたはスペース (ddd-dd-dddd または ddd dd dddd) の形式になっています。
    
  - Func_randomized_unformatted_ssn は、2011 年以降の SSN を検索します。これは 9 桁の連続した数字 (ddddddddd) の形式になっています。
    
- **[チェックサム:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** いいえ、チェックサムはありません。 
    
- **[定義:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP ポリシーは、抽出した約 300 文字が次の条件に該当することを検出した場合に、85% の確証を持ってそれがこの種類の機密情報であると特定します。 
    
  - [関数 Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) がパターンに一致するコンテンツを検出した。 
    
  - [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) から 1 つのキーワードが見つかった。キーワードの例には、*Social Security、Social Security#、Soc Sec、SSN* が含まれます。たとえば、**SSN: 489-36-8350** は DLP SSN ポリシーをトリガーします。
    
コンテンツに対して SSN を検出するために必要なものに関する詳細については、この記事の「[SSN に関する機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)」を参照してください。
  
さまざまな組み込みの機密情報の種類を使用している場合は、「[機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)」の記事でその他の種類に必要なものを参照してください。
  


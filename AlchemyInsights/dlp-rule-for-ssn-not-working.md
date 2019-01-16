---
title: SSN が動作していないため、DLP ルール
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297281"
---
**データ損失防止 (DLP)** を Office 365 で機密性の高い情報の種類を使用する場合、**社会保障番号 (SSN)** が含まれているコンテンツの動作していない問題が発生しているでしょうか。場合は、コンテンツには、DLP ポリシーが目的に必要な情報が含まれていることを確認します。 
  
など、ssn 型は、85% の信頼レベルで構成されているポリシーを次は評価されて、ルールをトリガーするを検出する必要があります。
  
- **[形式:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 桁、またはフォーマットしていないパターンである可能性があります。 
    
- **[パターン:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 4 つの関数は、次の 4 つの異なるパターンで、Ssn を検索します。 
    
  - Func_ssn は 2011 年以前の、厳密な書式の SSN を検索します。これはダッシュまたはスペース (ddd-dd-dddd または ddd dd dddd) の形式になっています。
    
  - Func_unformatted_ssn は 2011 年以前の、厳密な書式の SSN を検索します。これは 9 桁の連続した数字 (ddddddddd) の形式になっています。
    
  - Func_randomized_formatted_ssn は 2011 年以降の SSN を検索します。これはダッシュまたはスペース (ddd-dd-dddd または ddd dd dddd) の形式になっています。
    
  - Func_randomized_unformatted_ssn は 2011 年以降の SSN を検索します。これは 9 桁の連続した数字 (ddddddddd) の形式になっています。
    
- **[チェックサム:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** いいえ、チェックサムがないです。 
    
- **[定義:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP ポリシーとは、85% をこの種類の機密情報を検出したことを確信、近くにある 300 文字以内の場合。 
    
  - [関数 Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)では、パターンに一致するコンテンツを検索します。 
    
  - [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)からキーワードを検出するとします。キーワードの例が含まれています:*社会保障、社会保障番号、Soc 秒、SSN* 。SSN の DLP ポリシーの次の例では、たとえば、: **SSN: 489-36-8350**
    
Ssn をコンテンツの検出に必要なものの詳細については、この資料の次のセクションを参照してください:[どのような機密性の高い情報型 Ssn を検索](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
組み込まれている機密情報を別の型を使用して [その他の種類に必要なものについては、次の資料を参照してください:[どのような機密性の高い情報の種類を探します](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  


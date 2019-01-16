---
title: 動作していない米国の銀行口座番号の DLP ルール
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28298355"
---
**データ損失防止 (DLP)** O365 で DLP の機密性の高い情報の種類を使用する場合は、**米国の銀行口座番号**を含むコンテンツの動作していない問題が発生しているでしょうか。場合は、確認してください、コンテンツが含まれています DLP ポリシーは、探しているものが評価されるときに必要な情報にはです。 
  
などの 85% の信頼レベルで構成されているポリシーの**米国の銀行口座番号**、次は評価され、ルールをトリガーするを検出する必要があります。 
  
- **[形式:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 桁の数字 
    
- **[パターン:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 の連続した数字です。 
    
- **[チェックサム:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** いいえ、チェックサムがないです。 
    
- **[定義:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP ポリシーとは、75% が確実にこのような機密性の高い情報が検出されたが、近くにある 300 文字以内の場合。 
    
  - Regex_usa_bank_account_number の正規表現パターンに一致するコンテンツを検索します。
    
  - Keyword_usa_Bank_Account のキーワードを検出した。
    
    **米国の銀行口座番号**のポリシーの次の例では、たとえば、: 当座預金口座 78344011 
    
**米国の銀行口座番号**をコンテンツの検出に必要なものの詳細については、この資料の次のセクションを参照してください:[どのような機密性の高い情報の種類](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
組み込まれている機密情報を別の型を使用して [その他の種類に必要なものについては、次の資料を参照してください:[どのような機密性の高い情報の種類を探します](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  


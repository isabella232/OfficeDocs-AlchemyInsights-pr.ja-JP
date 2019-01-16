---
title: 動作していないクレジット カード番号の DLP ルール
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297399"
---
**データ損失防止 (DLP)** O365 で DLP の機密性の高い情報の種類を使用する場合は、**クレジット カード番号**を含むコンテンツの動作していない問題が発生しているでしょうか。その場合は、コンテンツには、トリガーに必要な情報が含まれていることを確認して、DLP ポリシーが評価されるときです。などの 85% の信頼レベルで構成されている**クレジット カードのポリシー** 、次は評価され、ルールをトリガーするを検出する必要があります。 
  
- **[形式:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 桁の数字書式を設定することができますが、または書式設定されていない (dddddddddddddddd) と、Luhn のテストに合格する必要があります。 
    
- **[パターン:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Visa、Mastercard、カードの検出、安全、アメリカン エキスプレス、ギフト カード、および給仕のカードを含め、全世界のすべての主要ブランドからカードを検出する非常に複雑で堅牢なパターンです。 
    
- **[チェックサム:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** はい、Luhn のチェックサム 
    
- **[定義:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP ポリシーとは、85% をこの種類の機密情報を検出したことを確信、近くにある 300 文字以内の場合。 
    
  - 関数 Func_credit_card がパターンに一致するコンテンツを検出した。
    
  - 次のいずれかの条件に該当する: 
    
  - Keyword_cc_verification のキーワードを検出した。
    
  - Keyword_cc_name からキーワードが見つかりました
    
  - 関数 Func_expiration_date が適切な日付形式の日付を検出した。
    
  - チェックサム パス
    
    たとえば、次の例を DLP のクレジット カード番号のポリシーのトリガー。
    
  - Visa: 4485 3647 3952 の 7352 
    
  - 有効期限: 2009 年 2 月
    
**クレジット カード番号**をコンテンツの検出に必要なものの詳細については、この資料の次のセクションを参照してください:[どのような機密性の高い情報の種類のクレジット カード番号の確認](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
組み込まれている機密情報を別の型を使用して [その他の種類に必要なものについては、次の資料を参照してください:[どのような機密性の高い情報の種類を探します](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  


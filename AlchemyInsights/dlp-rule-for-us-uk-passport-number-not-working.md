---
title: 米国の DLP ルールと動作していない、英国パスポート番号
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477112"
---
**データ損失防止 (DLP)** のコンテンツが含まれているために動作していない問題が発生している、**米国と英国のパスポート番号**O365 で DLP の機密性の高い情報の種類を使用する場合でしょうか。場合は、確認してください、コンテンツが含まれています DLP ポリシーは、探しているものが評価されるときに必要な情報にはです。 
  
などの**米国と英国のパスポート番号**の 75% の信頼レベルで構成されているポリシーは、次は評価され、ルールをトリガーするを検出する必要があります 
  
- **[形式:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 9 桁 
    
- **[パターン:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 9 つの連続した数字 
    
- **[チェックサム:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** いいえ、チェックサムがないです。 
    
- **[定義:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP ポリシーとは、75% が確実にこのような機密性の高い情報が検出されたが、近くにある 300 文字以内の場合。 
    
  - 関数 Func_usa_uk_passport がパターンに一致するコンテンツを検出した。
    
  - Keyword_passport のキーワードを検出した。
    
    次の例では、たとえば、**米国と英国のパスポート番号**ポリシー: u. s. パスポート番号 123456789 
    
米国に必要なものの詳細については、コンテンツのために認識されるようにイギリスのパスポート番号は、この資料の次のセクションを参照してください/:[ではどのような機密性の高い情報の種類の外観と英国のパスポート番号](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
組み込まれている機密情報を別の型を使用して [その他の種類に必要なものについては、次の資料を参照してください:[どのような機密性の高い情報の種類を探します](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  


---
title: 米国の銀行口座番号の DLP ルールが機能しない場合
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916421"
---
Office 365 で DLP 機密情報の種類を使用しているときに、**米国の銀行口座番号**を含むコンテンツに対して**データ損失防止 (DLP)** が機能しないという問題が発生した場合は、DLP ポリシーに必要な情報がコンテンツに含まれていることを確認してください。 
  
たとえば、85% の信頼レベルで構成された**米国の銀行口座番号**では、以下の内容が評価されるため、ルールをトリガーするためにはこれらの内容が検出される必要があります。 
  
- **[書式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8 ～ 17 桁の数字 
    
- **[パターン:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8 ～ 17 桁の連続する数字。 
    
- **[チェックサム:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** いいえ、チェックサムはありません。 
    
- **[定義:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP ポリシーは、抽出した約 300 文字が次の条件に該当することを検出した場合に、75% の確証を持ってそれがこの種類の機密情報であると特定します。 
    
  - 正規表現 Regex_usa_bank_account_number がパターンに一致するコンテンツを検出した
    
  - Keyword_usa_Bank_Account のキーワードを検出した。
    
    たとえば、次の当座預金口座 78344011 では、**米国の銀行口座番号** のポリシーがトリガーされます。 
    
コンテンツに対して**米国の銀行口座番号**が検出されるために必要な情報の詳細については、この記事の「[米国の銀行口座番号 SSN に関する機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)」を参照してください。
  
さまざまな組み込みの機密情報の種類を使用している場合は、「[機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)」の記事でその他の種類に必要なものを参照してください。
  


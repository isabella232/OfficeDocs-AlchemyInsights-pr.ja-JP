---
title: US/UK パスポート番号の DLP ルールが機能しない
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912106"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP の問題 - US/UK パスポート番号

Office 365 で DLP 機密情報の種類を使用しているときに、**US/UK パスポート番号**を含むコンテンツに対して**データ損失防止 (DLP)** が機能しないという問題が発生した場合は、DLP ポリシーに必要な情報がコンテンツに含まれていることを確認してください。 
  
たとえば、75% の信頼レベルで構成された **US/UK パスポート番号**では、以下の内容が評価されるため、ルールをトリガーするためにはこれらの内容が検出される必要があります 
  
- **[書式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 9 桁の数字 
    
- **[パターン:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 9 桁の連続する数字 
    
- **[チェックサム:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** いいえ、チェックサムはありません 
    
- **[定義:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP ポリシーは、抽出した約 300 文字が次の条件に該当することを検出した場合に、75% の確証を持ってそれがこの種類の機密情報であると特定します。 
    
  - 関数 Func_usa_uk_passport がパターンに一致するコンテンツを検出した。
    
  - Keyword_passport のキーワードを検出した。
    
    たとえば、次のサンプルでは **US/UK パスポート番号**ポリシー (U.S. Passport number 123456789) をトリガーします。 
    
コンテンツに対して US/UK パスポート番号が検出されるために必要な情報の詳細については、この記事の「[US/UK パスポート番号に関する機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)」セクションを参照してください。
  
さまざまな組み込みの機密情報の種類を使用している場合は、「[機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)」の記事でその他の種類に必要なものを参照してください。
  


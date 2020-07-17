---
title: クレジット カード番号の DLP ルールが機能しない
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507411"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>クレジット カード番号に関する DLP 問題

**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。

**クレジット カード番号に関する DLP 問題**

O365 で機密情報の種類 DLP を使用しているときに、**クレジット カード番号**を含むコンテンツに対して**データ損失防止 (DLP)** が機能しないという問題が発生する場合があります。その場合は、評価時に DLP ポリシーをトリガーするのに必要な情報がコンテンツに含まれていることを確認してください。たとえば、85% の信頼レベルで構成されている**クレジット カード ポリシー**の場合は、ルールをトリガーするために以下が評価され、検出される必要があります。
  
- **[書式:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 書式設定あり、または書式設定なし (dddddddddddddddd) の 16 桁の数字 (Luhn テストに合格する必要あり)。

- **[パターン:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** 世界規模の主要ブランドのカード (Visa、MasterCard、Discover Card、JCB、American Express、ギフト カード、Dinars Club Card など) を検出する非常に複雑で信頼性の高いパターンです。

- **[チェックサム:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** あり (Luhn のチェックサム)。

- **[定義:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP ポリシーは、抽出した約 300 文字が次の条件に該当することを検出した場合に、85% の確証を持ってそれがこの種類の機密情報であると特定します。

  - 関数 Func_credit_card がパターンに一致するコンテンツを検出した。

  - 次のいずれかの条件に該当する:

  - Keyword_cc_verification のキーワードを検出した。

  - Keyword_cc_name のキーワードを検出した。

  - 関数 Func_expiration_date が適切な日付形式の日付を検出した。

  - チェックサムが渡される。

    たとえば、次の例は DLP クレジット カード番号ポリシーに対してトリガーされます。

  - Visa: 4485 3647 3952 7352
  
  - 有効期限: 2/2009

コンテンツに対して**クレジット カード番号**を検出するために必要なものに関する詳細については、この記事の「[What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)」(クレジット カード番号に関する機密情報の種類の検索基準) を参照してください。
  
さまざまな組み込みの機密情報の種類を使用している場合は、「[機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)」の記事でその他の種類に必要なものを参照してください。
  